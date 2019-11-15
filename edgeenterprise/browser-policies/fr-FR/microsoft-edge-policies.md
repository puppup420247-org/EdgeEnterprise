---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 11/13/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge - Stratégies
La dernière version de Microsoft Edge inclut les stratégies suivantes. Vous pouvez utiliser ces stratégies pour configurer l’exécution de Microsoft Edge au sein de votre organisation.

Pour plus d’informations sur un ensemble de stratégies supplémentaires utilisées pour contrôler le mode et le moment de mise à jour de Microsoft Edge, consultez [Référence de la stratégie de mise à jour Microsoft Edge](microsoft-edge-update-policies.md)

> [!REMARQUE]
> Cet article s’applique à Microsoft Edge version 77 ou ultérieure.

## Stratégies disponibles
Ces tableaux répertorient toutes les stratégies de groupe liées au navigateur disponibles dans cette version de Microsoft Edge. Utilisez les liens de la table pour obtenir plus de détails sur les stratégies spécifiques.

|||
|-|-|
|[Authentification HTTP](#authentification-http)|[Cast](#cast)|
|[Démarrage, page d’accueil et page Nouvel onglet](#démarrage-page-d’accueil-et-page-nouvel-onglet)|[Extensions](#extensions)|
|[Gestionnaire de mot de passe et protection](#gestionnaire-de-mot-de-passe-et-protection)|[Impression](#impression)|
|[Messagerie native](#messagerie-native)|[Moteur de recherche par défaut](#moteur-de-recherche-par-défaut)|
|[Paramètres de SmartScreen](#paramètres-de-smartscreen)|[Paramètres de contenu](#paramètres-de-contenu)|
|[Serveur proxy](#serveur-proxy)|[Additional](#additional)|


### [*Authentification HTTP*](#authentification-http-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|Autoriser les invites d’authentification de base HTTP cross-origin|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Spécifie la liste des serveurs auxquels Microsoft Edge peut déléguer des identifiants utilisateur|
|[AuthSchemes](#authschemes)|Schémas d’authentification pris en charge|
|[AuthServerAllowlist](#authserverallowlist)|Configurer la liste des serveurs d’authentification autorisés|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|Désactiver la recherche CNAME lors de la négociation de l’authentification Kerberos|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Inclure le port non standard dans Kerberos SPN|
|[NtlmV2Enabled](#ntlmv2enabled)|Contrôler si l’authentification NTLMv2 est activée|
### [*Cast*](#cast-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Activer Google Cast|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|Afficher l’icône de diffusion dans la barre d’outils|
### [*Démarrage&comma; page d’accueil et page Nouvel onglet*](#démarrage-page-d’accueil-et-page-nouvel-onglet-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|Définir la page Nouvel onglet comme page d’accueil|
|[HomepageLocation](#homepagelocation)|Configurer l’URL de la page d’accueil|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|Définir le logo d'entreprise de l'onglet Nouveau|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|Masquer les sites populaires par défaut à partir du nouvel onglet|
|[NewTabPageLocation](#newtabpagelocation)|Configurer l’URL du nouvel onglet|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|Définir les liens rapides du nouvel onglet|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Configurer l’expérience de nouvel onglet Microsoft Edge|
|[RestoreOnStartup](#restoreonstartup)|Action à exécuter au démarrage|
|[RestoreOnStartupURLs](#restoreonstartupurls)|Sites à ouvrir au démarrage du navigateur|
|[ShowHomeButton](#showhomebutton)|Afficher le bouton Accueil sur la barre d’outils|
### [*Extensions*](#extensions-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|Configurer les types d’extensions autorisées|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|Autoriser l'installation d'extensions spécifiques|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|Contrôler les extensions impossibles à installer|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|Contrôler les extensions qui sont installées en mode silencieux|
|[ExtensionInstallSources](#extensioninstallsources)|Configurer l’extension et les sources d’installation du script utilisateur|
|[ExtensionSettings](#extensionsettings)|Configurer les paramètres de gestion des extensions|
### [*Gestionnaire de mot de passe et protection*](#gestionnaire-de-mot-de-passe-et-protection-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|Activer l’enregistrement des mots de passe pour le Gestionnaire de mot de passe|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|Configurer l’URL de modification du mot de passe|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|Configurer la liste des URL de connexion d’entreprise où le service de protection par mot de passe doit capturer l’empreinte digitale du mot de passe|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|Configurer le déclencheur d'avertissement de protection par mot de passe|
### [*Impression*](#impression-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|Règles de sélection d’imprimante par défaut|
|[PrintHeaderFooter](#printheaderfooter)|Imprimer des en-têtes et des pieds de page|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|Définir l’imprimante système par défaut en tant qu’imprimante par défaut|
|[PrintingEnabled](#printingenabled)|Activer l’impression|
|[UseSystemPrintDialog](#usesystemprintdialog)|Imprimer à l’aide de la boîte de dialogue d’impression système|
### [*Messagerie native*](#messagerie-native-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|Contrôle des hôtes de messagerie natifs pouvant être utilisés par les utilisateurs|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|Configurer la liste rouge de messagerie native|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|Autoriser les hôtes de messagerie natifs au niveau de l’utilisateur (installés sans autorisation d’administrateur)|
### [*Moteur de recherche par défaut*](#moteur-de-recherche-par-défaut-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|Activer le moteur de recherche par défaut|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|Encodages du moteur de recherche par défaut|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|Spécifie la fonction de recherche-par-image pour le moteur de recherche par défaut|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|Paramètres pour une URL d’image qui utilise POST|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|Mot clé du moteur de recherche par défaut|
|[DefaultSearchProviderName](#defaultsearchprovidername)|Nom du moteur de recherche par défaut|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|URL de recherche du moteur de recherche par défaut|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|URL du moteur de recherche par défaut pour les suggestions|
### [*Paramètres de SmartScreen*](#paramètres-de-smartscreen-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|Empêcher le contournement des avertissements de Microsoft Defender SmartScreen pour les sites|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|Empêcher le contournement des avertissements de Microsoft Defender SmartScreen concernant les téléchargements|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Configurer la liste des domaines pour lesquels Microsoft Defender SmartScreen ne déclenche pas d'avertissement|
|[SmartScreenEnabled](#smartscreenenabled)|Configurer Microsoft Defender SmartScreen|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|Forcer les vérifications de Microsoft Defender SmartScreen sur les téléchargements provenant de sources approuvées|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Configure Microsoft Defender SmartScreen to block potentially unwanted apps|
### [*Paramètres de contenu*](#paramètres-de-contenu-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|Sélectionner automatiquement des certificats clients pour ces sites|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|Autoriser les cookies sur des sites spécifiques|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|Bloquer les cookies sur des sites spécifiques|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|Limiter les cookies provenant de sites web spécifiques à la session active|
|[DefaultCookiesSetting](#defaultcookiessetting)|Configurer les cookies|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|Paramètre de géolocalisation par défaut|
|[DefaultImagesSetting](#defaultimagessetting)|Paramètres des images par défaut|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|Paramètre par défaut de JavaScript|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|Paramètres de notification par défaut|
|[DefaultPluginsSetting](#defaultpluginssetting)|Paramètre Adobe Flash par défaut|
|[DefaultPopupsSetting](#defaultpopupssetting)|Paramètres de fenêtre contextuelle par défaut|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Contrôler l’utilisation de l’API web Bluetooth|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|Contrôler l’utilisation de l’API WebUSB|
|[ImagesAllowedForUrls](#imagesallowedforurls)|Autoriser les images sur ces sites|
|[ImagesBlockedForUrls](#imagesblockedforurls)|Bloquer les images sur des sites spécifiques|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|Autoriser JavaScript sur des sites spécifiques|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|Bloquer JavaScript sur des sites spécifiques|
|[LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)|Enable default legacy SameSite cookie behavior setting|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](#legacysamesitecookiebehaviorenabledfordomainlist)|Revert to legacy SameSite behavior for cookies on specified sites|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|Autoriser les notifications sur des sites spécifiques|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|Bloquer les notifications sur des sites spécifiques|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|Autoriser le plug-in Adobe Flash sur des sites spécifiques|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|Bloquer le plug-in Adobe Flash sur des sites spécifiques|
|[PopupsAllowedForUrls](#popupsallowedforurls)|Autoriser les fenêtres contextuelles sur des sites spécifiques|
|[PopupsBlockedForUrls](#popupsblockedforurls)|Bloquer les fenêtres contextuelles sur des sites spécifiques|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|Inscrire les gestionnaires de protocole|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|Accorder l’accès à des sites spécifiques pour se connecter à des périphériques USB spécifiques|
|[WebUsbAskForUrls](#webusbaskforurls)|Autoriser WebUSB sur des sites spécifiques|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|Bloquer WebUSB sur des sites spécifiques|
### [*Serveur proxy*](#serveur-proxy-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[ProxyBypassList](#proxybypasslist)|Configurer les règles de contournement du proxy|
|[ProxyMode](#proxymode)|Configurer les paramètres du serveur proxy|
|[ProxyPacUrl](#proxypacurl)|Définir l'URL du fichier .pac du proxy|
|[ProxyServer](#proxyserver)|Configurer l’adresse ou l’URL du serveur proxy|
|[ProxySettings](#proxysettings)|Paramètres du proxy|
### [*Additional*](#additional-policies)
|Nom de la stratégie|Sous-titre|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|Paramètres des annonces pour les sites contenant des annonces gênantes|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|Activer la suppression de l'historique du navigateur et des téléchargements|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|Boîtes de dialogue Autoriser la sélection de fichiers|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|Autorise une page à afficher les fenêtres contextuelles pendant son déchargement|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|Autoriser les pages à envoyer des demandes XHR synchrones lors de l’opération de rejet de page|
|[AllowTrackingForUrls](#allowtrackingforurls)|Configurer les exceptions de prévention du suivi pour des sites spécifiques|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|Toujours ouvrir les fichiers PDF en externe|
|[ApplicationLocaleValue](#applicationlocalevalue)|Définir les paramètres régionaux de l'application|
|[AudioCaptureAllowed](#audiocaptureallowed)|Autoriser ou bloquer la capture audio|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|Sites pouvant accéder aux appareils de capture audio sans demander l’autorisation|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|Importer automatiquement les données et les paramètres d’un autre navigateur lors de la première exécution|
|[AutofillAddressEnabled](#autofilladdressenabled)|Activer le remplissage auto pour les adresses|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|Activer le Remplissage auto pour les cartes de crédit|
|[AutoplayAllowed](#autoplayallowed)|Autoriser la lecture automatique de média pour les sites web|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Poursuivre l’exécution des applications en arrière-plan après la fermeture de Microsoft Edge|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|Active les mises à jour en arrière-plan dans la liste des modèles disponibles pour les collections et d’autres fonctionnalités qui utilisent des modèles.|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|Bloquer les cookies tiers|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|Activer la création de profil à partir du menu déroulant Identité ou de la page Paramètres|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|Activer le mode invité|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|Autoriser les requêtes auprès d'un service de temps réseau de navigateur|
|[BrowserSignin](#browsersignin)|Paramètres de connexion du navigateur|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|Utiliser le client DNS intégré|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|Désactiver l'application transparence de certificat pour la liste des hachages subjectPublicKeyInfo|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|Désactivez l’application de transparence de certificat pour obtenir la liste des autorités de certification héritées|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|Désactiver l'application de transparence de certificat pour des URL spécifiques|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Effacer les données de navigation à la fermeture de Microsoft Edge|
|[ClickOnceEnabled](#clickonceenabled)|Autoriser les utilisateurs à ouvrir des fichiers à l’aide du protocole ClickOnce|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|Activer les avertissements de sécurité pour les indicateurs de ligne de commande|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Activer les mises à jour de composant dans Microsoft Edge|
|[ConfigureDoNotTrack](#configuredonottrack)|Configurer Ne pas me suivre|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|Configuration la conversion de texte par synthèse vocale en ligne|
|[CustomHelpLink](#customhelplink)|Spécifier le lien d’aide personnalisé|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Définir Microsoft Edge comme navigateur par défaut|
|[DeveloperToolsAvailability](#developertoolsavailability)|Contrôler où les outils de développement peuvent être utilisés|
|[DirectInvokeEnabled](#directinvokeenabled)|Autoriser les utilisateurs à ouvrir des fichiers à l’aide du protocole DirectInvoke|
|[Disable3DAPIs](#disable3dapis)|Désactiver la prise en charge des API graphiques 3D|
|[DisableScreenshots](#disablescreenshots)|Désactiver la création de captures d’écran|
|[DiskCacheDir](#diskcachedir)|Définir le répertoire du cache du disque|
|[DiskCacheSize](#diskcachesize)|Définir la taille de cache du disque, en octets|
|[DownloadDirectory](#downloaddirectory)|Définir le répertoire de téléchargement|
|[DownloadRestrictions](#downloadrestrictions)|Autoriser les restrictions de téléchargement|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|Activer la fonctionnalité Collections|
|[EditFavoritesEnabled](#editfavoritesenabled)|Autorise les utilisateurs à modifier les favoris|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|Réactiver les fonctionnalités de plateforme web déconseillées pendant une durée limitée|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|Activer le téléchargement des actions de domaine à partir de Microsoft|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|Activer les contrôles de protocole OCSP/liste de révocation de certificats en ligne|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|Autoriser les extensions managées de manière à utiliser l’API de plateforme de matériel d’entreprise|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|Contrôler la communication avec le service d’expérimentation et de configuration|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Afficher une case à cocher « Toujours ouvrir » dans la boîte de dialogue de protocole externe.|
|[FavoritesBarEnabled](#favoritesbarenabled)|Activer la barre des favoris|
|[ForceBingSafeSearch](#forcebingsafesearch)|Appliquer la recherche sécurisée Bing|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|Activer l’utilisation des profils éphémères|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Appliquer Google SafeSearch|
|[ForceNetworkInProcess](#forcenetworkinprocess)|Forcer le code de mise en réseau à s’exécuter dans le processus du navigateur|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|Forcer le mode Limité YouTube minimal|
|[FullscreenAllowed](#fullscreenallowed)|Autoriser le mode plein écran|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|Force la navigation directe sur un site intranet au lieu de rechercher des entrées à mots uniques dans la barre d’adresses|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|Configurez la liste des noms qui vont contourner la vérification de stratégie HSTS|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|Utiliser l’accélération matérielle (si disponible)|
|[ImportAutofillFormData](#importautofillformdata)|Autoriser l’importation des données du formulaire de remplissage auto|
|[ImportBrowserSettings](#importbrowsersettings)|Autoriser l’importation des paramètres du navigateur|
|[ImportFavorites](#importfavorites)|Autoriser l’importation des favoris|
|[ImportHistory](#importhistory)|Autoriser l’importation de l’historique de navigation|
|[ImportHomepage](#importhomepage)|Autoriser l’importation des paramètres de la page d’accueil|
|[ImportOpenTabs](#importopentabs)|Autoriser l’importation des onglets ouverts|
|[ImportPaymentInfo](#importpaymentinfo)|Autoriser l’importation des infos de paiement|
|[ImportSavedPasswords](#importsavedpasswords)|Autoriser l’importation des mots de passe enregistrés|
|[ImportSearchEngine](#importsearchengine)|Autoriser l’importation des paramètres du moteur de recherche|
|[InPrivateModeAvailability](#inprivatemodeavailability)|Configurer la disponibilité du mode InPrivate|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Configurer l’intégration d’Internet Explorer|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|Configurer la liste des sites en Mode entreprise|
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Spécifier le type de comportement des navigations « entre les pages » vers des sites non configurés lorsqu’elles commencent sur des pages en mode Internet Explorer|
|[IsolateOrigins](#isolateorigins)|Activer l’isolation de site pour des origines spécifiques|
|[ManagedFavorites](#managedfavorites)|Configurer les favoris|
|[ManagedSearchEngines](#managedsearchengines)|Gérer les moteurs de recherche|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|Nombre maximal de connexions simultanées au serveur proxy|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Autoriser Google Cast à se connecter aux appareils Cast sur toutes les adresses IP|
|[MetricsReportingEnabled](#metricsreportingenabled)|Activer l’utilisation et les rapports de données liées à l’incident|
|[NetworkPredictionOptions](#networkpredictionoptions)|Activer la prédiction réseau|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|Configurer si un utilisateur dispose toujours d’un profil par défaut connecté automatiquement avec son compte professionnel ou scolaire|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|Contrôler l’application des restrictions de sécurité aux origines non sécurisées|
|[ProactiveAuthEnabled](#proactiveauthenabled)|Activer l’authentification proactive|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|Autoriser le contenu promotionnel dans des onglets|
|[PromptForDownloadLocation](#promptfordownloadlocation)|Demander où enregistrer les fichiers téléchargés|
|[QuicAllowed](#quicallowed)|Autoriser le protocole QUIC|
|[RelaunchNotification](#relaunchnotification)|Avertir un utilisateur qu’un redémarrage du navigateur est recommandé ou requis pour les mises à jour en attente|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|Définir la période pour les notifications de mise à jour|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|Activer l’intégrité du code de rendu|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|Spécifier si des vérifications OCSP/liste de révocation de certificats en ligne sont obligatoires pour les ancres d’approbation locales|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|Activer la résolution des erreurs de navigation à l'aide d'un service web|
|[RestrictSigninToPattern](#restrictsignintopattern)|Restreindre les comptes qui peuvent être utilisés en tant que comptes principaux Microsoft Edge|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Étendre le paramètre de contenu d'Adobe Flash à l'ensemble du contenu|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|Autoriser les utilisateurs à continuer à partir de la page d’avertissement HTTPS|
|[SSLVersionMin](#sslversionmin)|Version TLS minimale activée|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|Désactiver l’enregistrement de l’historique du navigateur|
|[SearchSuggestEnabled](#searchsuggestenabled)|Activer les suggestions de recherche|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|Sites web ou domaines qui ne nécessitent pas l'autorisation d'utiliser l’attestation de clé de sécurité directe|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|Envoyer tous les sites intranet vers Internet Explorer|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Envoyer les informations de site pour améliorer les services Microsoft|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|Afficher les raccourcis Microsoft Office dans la barre des favoris|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|Activer la prise en charge de SXG (échange HTTP signé)|
|[SitePerProcess](#siteperprocess)|Activer l’isolation de site pour chaque site|
|[SpellcheckEnabled](#spellcheckenabled)|Activer la vérification orthographique|
|[SpellcheckLanguage](#spellchecklanguage)|Activer des langues de vérification orthographique spécifiques|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|Forcer la désactivation des langues de la vérification orthographique|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|Supprimer l’avertissement de système d’exploitation non pris en charge|
|[SyncDisabled](#syncdisabled)|Désactiver la synchronisation des données à l’aide des services de synchronisation Microsoft|
|[TabFreezingEnabled](#tabfreezingenabled)|Autoriser le gel des onglets d’arrière-plan|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|Activer la fin des processus dans le gestionnaire des tâches du navigateur|
|[TrackingPrevention](#trackingprevention)|Bloquer le suivi de l’activité de navigation sur le Web des utilisateurs|
|[TranslateEnabled](#translateenabled)|Activer Traduire|
|[URLAllowlist](#urlallowlist)|Définir une liste d’URL autorisées|
|[URLBlocklist](#urlblocklist)|Bloquer l’accès à une liste d’URL|
|[UserDataDir](#userdatadir)|Définir le répertoire des données utilisateur|
|[UserFeedbackAllowed](#userfeedbackallowed)|Autoriser les commentaires des utilisateurs|
|[VideoCaptureAllowed](#videocaptureallowed)|Autoriser ou bloquer la capture vidéo|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|Sites pouvant accéder aux appareils de capture vidéo sans demander l’autorisation|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|Définir l'optimisation WPAD|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|Autoriser WebDriver à remplacer les stratégies incompatibles|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Limiter l’exposition de l’adresse IP localhost par WebRTC|
|[WebRtcUdpPortRange](#webrtcudpportrange)|Limiter la plage de ports UDP locaux utilisés par WebRTC|




  ## Authentification HTTP policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### AllowCrossOriginAuthPrompt
  #### Autoriser les invites d’authentification de base HTTP cross-origin
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôle si le contenu secondaire tiers sur une page peut ouvrir une boîte de dialogue d’authentification de base HTTP.

En règle générale, cette option est désactivée pour une protection contre le hameçonnage. Si vous ne configurez pas cette stratégie, elle est désactivée et le contenu secondaire tiers ne peut pas ouvrir une boîte de dialogue d’authentification de base HTTP.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AllowCrossOriginAuthPrompt
  - Nom de la stratégie de groupe: Autoriser les invites d’authentification de base HTTP cross-origin
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Authentification HTTP
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AllowCrossOriginAuthPrompt
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AllowCrossOriginAuthPrompt
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AuthNegotiateDelegateAllowlist
  #### Spécifie la liste des serveurs auxquels Microsoft Edge peut déléguer des identifiants utilisateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configurer la liste des serveurs auxquels Microsoft Edge peut déléguer.

	Séparez plusieurs noms de serveurs par des virgules. Les caractères génériques (*) sont autorisés.

	Si vous ne configurez pas cette stratégie, Microsoft Edge ne peut pas déléguer les informations d’identification de l’utilisateur, même si un serveur est détecté comme intranet.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AuthNegotiateDelegateAllowlist
  - Nom de la stratégie de groupe: Spécifie la liste des serveurs auxquels Microsoft Edge peut déléguer des identifiants utilisateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Authentification HTTP
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AuthNegotiateDelegateAllowlist
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"contoso.com"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AuthNegotiateDelegateAllowlist
  - Exemple de valeur :
``` xml
<string>contoso.com</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AuthSchemes
  #### Schémas d’authentification pris en charge
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie les schémas d’authentification HTTP pris en charge.

Vous pouvez configurer la stratégie en utilisant les valeurs suivantes : « basic », « digest », « ntlm » et « negotiate ». Séparez plusieurs valeurs par des virgules.

Si vous ne configurez pas cette stratégie, les quatre modèles sont utilisés.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AuthSchemes
  - Nom de la stratégie de groupe: Schémas d’authentification pris en charge
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Authentification HTTP
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AuthSchemes
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"basic,digest,ntlm,negotiate"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AuthSchemes
  - Exemple de valeur :
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AuthServerAllowlist
  #### Configurer la liste des serveurs d’authentification autorisés
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie les serveurs à activer pour l’authentification intégrée. L’authentification intégrée n’est activée que lorsque Microsoft Edge reçoit une demande d’authentification à partir d’un proxy ou d’un serveur de cette liste.

	Séparez les noms de serveurs multiples par des virgules. Les caractères génériques (*) sont autorisés.

	Si vous ne configurez pas cette stratégie, Microsoft Edge essaie de détecter si un serveur se trouve sur l’intranet. Ce n'est qu'à ce moment-là qu’il répond aux requêtes IWA. Si le serveur se trouve sur Internet, les requêtes IWA émanant de celui-ci sont ignorées par Microsoft Edge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AuthServerAllowlist
  - Nom de la stratégie de groupe: Configurer la liste des serveurs d’authentification autorisés
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Authentification HTTP
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AuthServerAllowlist
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"*contoso.com,contoso.com"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AuthServerAllowlist
  - Exemple de valeur :
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DisableAuthNegotiateCnameLookup
  #### Désactiver la recherche CNAME lors de la négociation de l’authentification Kerberos
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Détermine si le SPN Kerberos généré est basé sur le nom DNS canonique (CNAME) ou sur le nom d’origine entré.

Si vous activez cette stratégie, la recherche CNAME est ignorée et le nom du serveur (tel qu'il a été entré) est utilisé.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, le nom canonique du serveur est utilisé. Ceci est déterminé via une recherche CNAME.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DisableAuthNegotiateCnameLookup
  - Nom de la stratégie de groupe: Désactiver la recherche CNAME lors de la négociation de l’authentification Kerberos
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Authentification HTTP
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DisableAuthNegotiateCnameLookup
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DisableAuthNegotiateCnameLookup
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### EnableAuthNegotiatePort
  #### Inclure le port non standard dans Kerberos SPN
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie si le SPN Kerberos généré doit inclure un port non standard.

Si vous activez cette stratégie et si un utilisateur inclut un port non standard (un port différent de 80 ou 443) dans une URL, ce port est inclus dans le SPN Kerberos généré.

Si vous ne configurez pas ou si vous désactivez cette stratégie, le SPN Kerberos généré n’inclut de port dans aucun cas.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EnableAuthNegotiatePort
  - Nom de la stratégie de groupe: Inclure le port non standard dans Kerberos SPN
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Authentification HTTP
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: EnableAuthNegotiatePort
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EnableAuthNegotiatePort
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NtlmV2Enabled
  #### Contrôler si l’authentification NTLMv2 est activée
  >Versions prises en charge : Microsoft Edge sur Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôle si NTLMv2 est activée.

Toutes les versions récentes des serveurs Samba et Windows prennent en charge NTLMv2. Vous ne devez désactiver NTLMv2 que pour résoudre les problèmes de compatibilité descendante, car elle réduit la sécurité de l’authentification.

Si vous ne configurez pas cette stratégie, NTLMv2 est activé par défaut.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  

  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NtlmV2Enabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Cast policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### EnableMediaRouter
  #### Activer Google Cast
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Activez cette stratégie pour activer Google Cast. Les utilisateurs seront en mesure de le lancer à partir du menu de l'application, des menus contextuels de page, des contrôles de media sur les sites sur lesquels Cast est activé, et de l'icône de la barre d'outils Cast (le cas échéant).

Désactivez cette stratégie pour désactiver Google Cast.

Par défaut, Google Cast est activé.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EnableMediaRouter
  - Nom de la stratégie de groupe: Activer Google Cast
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Cast
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: EnableMediaRouter
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EnableMediaRouter
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ShowCastIconInToolbar
  #### Afficher l’icône de diffusion dans la barre d’outils
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Set this policy to true to show the Cast toolbar icon on the toolbar or the overflow menu. Users won't be able to remove it.

If you don't configure this policy or if you disable it, users can pin or remove the icon by using its contextual menu.

If you've also set the [EnableMediaRouter](#enablemediarouter) policy to false, then this policy is ignored, and the toolbar icon isn't shown.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ShowCastIconInToolbar
  - Nom de la stratégie de groupe: Afficher l’icône de diffusion dans la barre d’outils
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Cast
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ShowCastIconInToolbar
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ShowCastIconInToolbar
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Démarrage&comma; page d’accueil et page Nouvel onglet policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### HomepageIsNewTabPage
  #### Définir la page Nouvel onglet comme page d’accueil
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configurer la page d’accueil par défaut dans Microsoft Edge. Vous pouvez définir la page d’accueil sur une URL spécifiée ou sur la page Nouvel onglet.

	Si vous activez cette stratégie, la page Nouvel onglet est toujours utilisée pour la page d’accueil et l’emplacement de l’URL de la page d’accueil est ignoré.

	Si vous désactivez cette stratégie, la page d’accueil de l’utilisateur ne peut pas être la page Nouvel onglet, sauf si l’URL est définie sur « edge://newtab ».

	Si elle n’est pas configurée, les utilisateurs peuvent choisir si la page Nouvel onglet est leur page d’accueil.

	Cette stratégie n'est disponible que sur les instances de Windows jointes à un domaine Microsoft Active Directory ou les instances de Windows 10 Professionnel ou Entreprise inscrites pour la gestion des appareils.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: HomepageIsNewTabPage
  - Nom de la stratégie de groupe: Définir la page Nouvel onglet comme page d’accueil
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: HomepageIsNewTabPage
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: HomepageIsNewTabPage
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### HomepageLocation
  #### Configurer l’URL de la page d’accueil
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configures the default home page URL in Microsoft Edge.

The home page is the page opened by the Home button. The pages that open on startup are controlled by the [RestoreOnStartup](#restoreonstartup) policies.

You can either set a URL here or set the home page to open the new tab page. If you select to open the new tab page, then this policy doesn't take effect.

If you enable this policy, users can't change their home page URL, but they can choose to use the new tab page as their home page.

If you disable or don't configure this policy, users can choose their own home page, as long as the [HomepageIsNewTabPage](#homepageisnewtabpage) policy isn't enabled.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: HomepageLocation
  - Nom de la stratégie de groupe: Configurer l’URL de la page d’accueil
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: HomepageLocation
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://www.contoso.com"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: HomepageLocation
  - Exemple de valeur :
``` xml
<string>https://www.contoso.com</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NewTabPageCompanyLogo
  #### Définir le logo d'entreprise de l'onglet Nouveau
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Spécifie le logo de la société à utiliser sur dans le nouvel onglet dans Microsoft Edge.

La stratégie doit être configurée en tant que chaîne qui exprime le(s) logo(s) au format JSON. Par exemple { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

Pour configurer cette stratégie, spécifiez l’URL à partir de laquelle Microsoft Edge peut télécharger le logo et son hachage de chiffrement (SHA-256), qui permet de vérifier l’intégrité du téléchargement. Le logo doit être au format PNG ou SVG et sa taille de fichier ne doit pas dépasser 16 Mo. Le logo est téléchargé et mis en cache. Il est retéléchargé à chaque modification de l’URL ou du hachage. L’URL doit être accessible sans authentification.

Le « default_logo » est obligatoire et est utilisé lorsqu’il n’y a pas d’image d’arrière-plan. Si « light_logo » est spécifié, il est utilisé lorsque le nouvel onglet de l’utilisateur a une image d’arrière-plan. Nous vous conseillons d’utiliser un logo horizontal avec un arrière-plan transparent aligné à gauche et centré verticalement. Le logo doit avoir une hauteur minimale de 32 pixels et des proportions de 1:1 à 4:1. Le « default_logo » doit avoir un contraste approprié avec un arrière-plan blanc/noir, tandis que le « light_logo » doit avoir un contraste correct par rapport à une image d’arrière-plan.

Si vous activez cette stratégie, Microsoft Edge télécharge et affiche le(s) logo(s) spécifié(s) sur le nouvel onglet. Les utilisateurs ne peuvent pas remplacer ni masquer le(s) logo(s).

Si vous désactivez cette stratégie ou si vous ne la configurez pas, Microsoft Edge n’affiche pas de logo de la société ni de logo Microsoft sur le nouvel onglet.

Pour obtenir de l’aide sur la détermination du hachage SHA-256, voir https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/get-filehash?view=powershell-6.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NewTabPageCompanyLogo
  - Nom de la stratégie de groupe: Définir le logo d'entreprise de l'onglet Nouveau
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: NewTabPageCompanyLogo
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
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


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NewTabPageCompanyLogo
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NewTabPageHideDefaultTopSites
  #### Masquer les sites populaires par défaut à partir du nouvel onglet
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Masque les sites populaires par défaut à partir du nouvel onglet dans Microsoft Edge.

Si vous définissez cette stratégie sur true, les vignettes de site populaire par défaut sont masquées.

Si vous définissez cette stratégie sur false ou si vous ne la configurez pas, les vignettes de site populaire par défaut restent visibles.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NewTabPageHideDefaultTopSites
  - Nom de la stratégie de groupe: Masquer les sites populaires par défaut à partir du nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: NewTabPageHideDefaultTopSites
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NewTabPageHideDefaultTopSites
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NewTabPageLocation
  #### Configurer l’URL du nouvel onglet
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configures the default URL for the new tab page.

This policy determines the page that's opened when new tabs are created (including when new windows are opened). It also affects the startup page if that's set to open to the new tab page.

This policy doesn't determine which page opens on startup; that's controlled by the [RestoreOnStartup](#restoreonstartup) policy. It also doesn’t affect the home page if that’s set to open to the new tab page.

If you don't configure this policy, the default new tab page is used.

If you configure this policy *and* the [NewTabPageSetFeedType](#newtabpagesetfeedtype) policy, this policy has precedence.

If an invalid URL is provided, new tabs will open about://blank.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NewTabPageLocation
  - Nom de la stratégie de groupe: Configurer l’URL du nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: NewTabPageLocation
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://www.fabrikam.com"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NewTabPageLocation
  - Exemple de valeur :
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NewTabPageManagedQuickLinks
  #### Définir les liens rapides du nouvel onglet
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Par défaut, Microsoft Edge affiche les liens rapides du nouvel onglet à partir des raccourcis ajoutés par l’utilisateur et des sites récurrents en fonction de l’historique de navigation. Grâce à cette stratégie, vous pouvez configurer jusqu’à trois vignettes de liens rapides sur le nouvel onglet, exprimées sous forme d’objet JSON :

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

Le champ « URL » est obligatoire ; les éléments « titre » et « épinglé » sont facultatifs. Si « titre » n’est pas spécifié, l’URL est utilisée comme titre par défaut. Si « épinglé » n’est pas spécifié, la valeur par défaut est false.

Microsoft Edge présente celles-ci dans l’ordre listé, de gauche à droite, avec toutes les vignettes épinglées affichées avant les vignettes non épinglées.

Si la stratégie est définie comme obligatoire, le champ « épinglé » est ignoré et toutes les vignettes sont épinglées. Les vignettes ne peuvent pas être supprimées par l’utilisateur et apparaissent toujours au début de la liste des liens rapides.

Si la stratégie est définie comme recommandée, les vignettes épinglées sont conservées dans la liste, mais l’utilisateur peut les modifier et les supprimer. Les vignettes de lien rapide qui ne sont pas épinglées se comportent comme des sites récurrents par défaut et sont exclues de la liste si d’autres sites web sont visités plus fréquemment. Lors de l’application de liens non épinglés via cette stratégie à un profil de navigateur existant, il est possible que les liens n’apparaissent pas du tout, selon la façon dont ils sont classés par rapport à l’historique de navigation de l’utilisateur.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NewTabPageManagedQuickLinks
  - Nom de la stratégie de groupe: Définir les liens rapides du nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: NewTabPageManagedQuickLinks
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
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


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NewTabPageManagedQuickLinks
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NewTabPageSetFeedType
  #### Configurer l’expérience de nouvel onglet Microsoft Edge
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Vous permet de choisir l’expérience de flux Microsoft News ou Office 365 pour le nouvel onglet.

Si vous définissez cette stratégie sur l'expérience de flux Microsoft News (0), les utilisateurs voient l’expérience de flux Microsoft News sur le nouvel onglet.

Si vous définissez cette stratégie sur l'expérience de flux Office 365 (1), les utilisateurs disposant d’une connexion au navigateur Azure Active Directory voient l’expérience de flux Office 365 sur le nouvel onglet.

Si vous désactivez cette stratégie ou si vous ne la configurez pas :

-Les utilisateurs disposant d’une connexion au navigateur Azure Active Directory se voient proposer l’expérience de flux de nouvel onglet Office 365, ainsi que l’expérience de flux de nouvel onglet standard.

-        Les utilisateurs sans connexion au navigateur Azure Active Directory voient l’expérience de nouvel onglet standard.

Si vous configurez cette stratégie *et* la stratégie [NewTabPageLocation](#newtabpagelocation), [NewTabPageLocation](#newtabpagelocation) est prioritaire.

Paramètre par défaut : désactivé ou non configuré.

* 0 = Expérience de flux Microsoft News

* 1 = Expérience de flux Office 365

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NewTabPageSetFeedType
  - Nom de la stratégie de groupe: Configurer l’expérience de nouvel onglet Microsoft Edge
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: NewTabPageSetFeedType
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NewTabPageSetFeedType
  - Exemple de valeur :
``` xml
<integer>0</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RestoreOnStartup
  #### Action à exécuter au démarrage
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifiez la façon dont Microsoft Edge se comporte lorsqu’il démarre.

	Si vous voulez qu'un nouvel onglet s'ouvre toujours ouvrir au démarrage, cliquez sur « Ouvrir un nouvel onglet » (5).

	Si vous voulez rouvrir des URL ouvertes lors de la dernière fermeture de Microsoft Edge, sélectionnez « Restaurer la dernière session » (1). La session de navigation est restaurée telle qu'elle était. Notez que cette option désactive certains paramètres qui s’appuient sur des sessions ou qui effectuent des actions à la fermeture (telles qu'effacer les données de navigation en quittant ou les cookies de session uniquement).

	Si vous voulez ouvrir un ensemble d’URL spécifique, cliquez sur « Ouvrir une liste d’URL » (4).

	La désactivation de ce paramètre revient à le laisser non configuré. Les utilisateurs peuvent le modifier dans Microsoft Edge.

	Cette stratégie n'est disponible que sur les instances de Windows jointes à un domaine Microsoft Active Directory ou sur les instances de Windows 10 Professionnel ou Entreprise inscrites pour la gestion des appareils.

	* 5 = Ouvrir un nouvel onglet

	* 1 = Restaurer la dernière session

	* 4 = Ouvrir une liste d’URL

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RestoreOnStartup
  - Nom de la stratégie de groupe: Action à exécuter au démarrage
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: RestoreOnStartup
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000004
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: RestoreOnStartup
  - Exemple de valeur :
``` xml
<integer>4</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RestoreOnStartupURLs
  #### Sites à ouvrir au démarrage du navigateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specify a list of websites to open automatically when the browser starts. If you don't configure this policy, no site is opened on startup.

This policy only works if you also set the [RestoreOnStartup](#restoreonstartup) policy to 'Open a list of URLs' (4).

This policy is only available on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RestoreOnStartupURLs
  - Nom de la stratégie de groupe: Sites à ouvrir au démarrage du navigateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé\RestoreOnStartupURLs
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: RestoreOnStartupURLs
  - Exemple de valeur :
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ShowHomeButton
  #### Afficher le bouton Accueil sur la barre d’outils
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Affiche le bouton Accueil dans la barre d'outils de Microsoft Edge.

	Activez cette stratégie pour toujours afficher le bouton Accueil. Désactivez-la pour ne jamais afficher le bouton.

	Si vous ne configurez pas la stratégie, les utilisateurs peuvent choisir s’il veulent afficher le bouton Accueil.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ShowHomeButton
  - Nom de la stratégie de groupe: Afficher le bouton Accueil sur la barre d’outils
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Démarrage, page d’accueil et page Nouvel onglet
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Démarrage, page d’accueil et page Nouvel onglet
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ShowHomeButton
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ShowHomeButton
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Extensions policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExtensionAllowedTypes
  #### Configurer les types d’extensions autorisées
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Controls which extension types can be installed and limits runtime access.

This setting defines the allowed types of extensions and which hosts they can interact with. The value is a list of strings, each of which should be one of the following: "extension", "theme", "user_script", and "hosted_app". See the Microsoft Edge extensions documentation for more information on these types.

Note that this policy also affects extensions to be force-installed by using [ExtensionInstallForcelist](#extensioninstallforcelist) policy.

If you enable this policy, only extensions that match a type in the list are installed.

If you don't configure this policy, no restrictions on the acceptable extension types are enforced.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExtensionAllowedTypes
  - Nom de la stratégie de groupe: Configurer les types d’extensions autorisées
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Extensions
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExtensionAllowedTypes
  - Exemple de valeur :
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExtensionInstallAllowlist
  #### Autoriser l'installation d'extensions spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Par défaut, toutes les extensions sont autorisées. Toutefois, si vous bloquez toutes les extensions en définissant la stratégie « ExtensionInstallBlockList » sur « * », les utilisateurs ne peuvent installer que les extensions définies dans cette stratégie.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExtensionInstallAllowlist
  - Nom de la stratégie de groupe: Autoriser l'installation d'extensions spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Extensions
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExtensionInstallAllowlist
  - Exemple de valeur :
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExtensionInstallBlocklist
  #### Contrôler les extensions impossibles à installer
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Répertoriez des extensions spécifiques que les utilisateurs ne peuvent PAS installer dans Microsoft Edge. Lorsque vous déployez cette stratégie, toutes les extensions de cette liste qui ont été installées précédemment sont désactivées et l’utilisateur ne peut pas les activer. Si vous supprimez un élément de la liste des extensions bloquées, cette extension est automatiquement réactivée partout où elle a déjà été installée.

	Utilisez « * » pour bloquer toutes les extensions qui ne sont pas répertoriées de façon explicite dans la liste verte.

	Si vous ne configurez pas cette stratégie, les utilisateurs peuvent installer toutes les extensions de Microsoft Edge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExtensionInstallBlocklist
  - Nom de la stratégie de groupe: Contrôler les extensions impossibles à installer
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Extensions
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExtensionInstallBlocklist
  - Exemple de valeur :
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExtensionInstallForcelist
  #### Contrôler les extensions qui sont installées en mode silencieux
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
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

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExtensionInstallForcelist
  - Nom de la stratégie de groupe: Contrôler les extensions qui sont installées en mode silencieux
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Extensions
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExtensionInstallForcelist
  - Exemple de valeur :
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExtensionInstallSources
  #### Configurer l’extension et les sources d’installation du script utilisateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define URLs that can install extensions and themes.

By default, users have to download a *.crx file for each extension or script they want to install, and then drag it onto the Microsoft Edge settings page. This policy lets specific URLs use install the extension or script for the user.

Each item in this list is an extension-style match pattern (see [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Users can easily install items from any URL that matches an item in this list. Both the location of the *.crx file and the page where the download is started from (in other words, the referrer) must be allowed by these patterns.

The [ExtensionInstallBlocklist](#extensioninstallblocklist) policy takes precedence over this policy. Any extensions that's on the block list won't be installed, even if it comes from a site on this list.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExtensionInstallSources
  - Nom de la stratégie de groupe: Configurer l’extension et les sources d’installation du script utilisateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Extensions
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExtensionInstallSources
  - Exemple de valeur :
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExtensionSettings
  #### Configurer les paramètres de gestion des extensions
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configurer les paramètres de gestion d’extension de Microsoft Edge.

	Cette stratégie contrôle plusieurs paramètres, y compris les paramètres contrôlés par des stratégies existantes relatives à l’extension. Cette stratégie remplace les stratégies héritées si les deux sont définies.

	Cette stratégie mappe un ID d’extension ou une URL de mise à jour avec sa configuration. Avec un ID d’extension, la configuration s’applique uniquement à l’extension spécifiée. Définissez une configuration par défaut pour l’ID spécial « * » à appliquer à toutes les extensions qui ne sont pas spécifiquement répertoriées dans cette stratégie. Avec une URL de mise à jour, la configuration s’applique à toutes les extensions avec l’URL de mise à jour exact indiqué dans le manifeste de cette extension, comme décrit dans [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExtensionSettings
  - Nom de la stratégie de groupe: Configurer les paramètres de gestion des extensions
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Extensions
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ExtensionSettings
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
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


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExtensionSettings
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Gestionnaire de mot de passe et protection policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### PasswordManagerEnabled
  #### Activer l’enregistrement des mots de passe pour le Gestionnaire de mot de passe
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Activez Microsoft Edge pour enregistrer les mots de passe utilisateur.

	Si vous activez cette stratégie, les utilisateurs peuvent enregistrer leurs mots de passe Microsoft Edge. Lors de leur prochaine visite du site, Microsoft Edge entre automatiquement le mot de passe.

	Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas enregistrer de nouveaux mots de passe, mais ils peuvent toujours utiliser les mots de passe enregistrés précédemment.

	Si vous activez ou désactivez cette stratégie, les utilisateurs ne peuvent pas la modifier ni la remplacer dans Microsoft Edge. Si vous ne la configurez pas, les utilisateurs peuvent enregistrer les mots de passe, ainsi que désactiver cette fonctionnalité.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PasswordManagerEnabled
  - Nom de la stratégie de groupe: Activer l’enregistrement des mots de passe pour le Gestionnaire de mot de passe
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Gestionnaire de mot de passe et protection
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Gestionnaire de mot de passe et protection
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: PasswordManagerEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PasswordManagerEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PasswordProtectionChangePasswordURL
  #### Configurer l’URL de modification du mot de passe
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configure l’URL de modification du mot de passe (schémas HTTP et HTTPS uniquement).

Le service de protection par mot de passe redirige les utilisateurs vers cette URL pour modifier leur mot de passe après l'affichage d'un avertissement dans le navigateur.

Si vous activez cette stratégie, le service de protection par mot de passe redirige les utilisateurs vers cette URL pour modifier leur mot de passe.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, le service de protection par mot de passe ne redirige pas les utilisateurs vers une URL de modification du mot de passe.

Cette stratégie est disponible uniquement sur les instances de Windows jointes à un domaine Microsoft Active Directory ou les instances de Windows 10 Professionnel ou Entreprise inscrites pour la gestion des appareils.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PasswordProtectionChangePasswordURL
  - Nom de la stratégie de groupe: Configurer l’URL de modification du mot de passe
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Gestionnaire de mot de passe et protection
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: PasswordProtectionChangePasswordURL
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://contoso.com/change_password.html"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PasswordProtectionChangePasswordURL
  - Exemple de valeur :
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PasswordProtectionLoginURLs
  #### Configurer la liste des URL de connexion d’entreprise où le service de protection par mot de passe doit capturer l’empreinte digitale du mot de passe
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configurer la liste des URL de connexion d’entreprise (schémas HTTP et HTTPs uniquement) lorsque Microsoft Edge doit capturer l’empreinte digitale des mots de passe et l’utiliser pour la détection de réutilisation de mot de passe.

Si vous activez cette stratégie, le service de protection par mot de passe capture les empreintes digitales des mots de passe sur les URL définies.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, aucune empreinte de mot de passe n’est capturée.

Cette stratégie n'est disponible que sur les instances de Windows jointes à un domaine Microsoft Active Directory ou les instances de Windows 10 Professionnel ou Entreprise inscrites pour la gestion des appareils.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PasswordProtectionLoginURLs
  - Nom de la stratégie de groupe: Configurer la liste des URL de connexion d’entreprise où le service de protection par mot de passe doit capturer l’empreinte digitale du mot de passe
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Gestionnaire de mot de passe et protection
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PasswordProtectionLoginURLs
  - Exemple de valeur :
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PasswordProtectionWarningTrigger
  #### Configurer le déclencheur d'avertissement de protection par mot de passe
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Allows you to control when to trigger password protection warning. Password protection alerts users when they reuse their protected password on potentially suspicious sites.

You can use the [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) policies to configure which passwords to protect.

Exemptions: Passwords for the sites listed in [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl), as well as for the sites listed in [SmartScreenAllowListDomains](#smartscreenallowlistdomains), will not trigger a password-protection warning.

Set to 'PasswordProtectionWarningOff' (0) to not show password protection warningss.

Set to 'PasswordProtectionWarningOnPasswordReuse' (1) to show password protection warnings when the user reuses their protected password on a non-whitelisted site.

If you disable or don't configure this policy, then the warning trigger is not shown.

* 0 = Password protection warning is off.

* 1 = Password protection warning is triggered by password reuse.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PasswordProtectionWarningTrigger
  - Nom de la stratégie de groupe: Configurer le déclencheur d'avertissement de protection par mot de passe
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Gestionnaire de mot de passe et protection
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: PasswordProtectionWarningTrigger
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PasswordProtectionWarningTrigger
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Impression policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultPrinterSelection
  #### Règles de sélection d’imprimante par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Remplace les règles de sélection d’imprimante par défaut de Microsoft Edge. Cette stratégie détermine les règles pour la sélection de l’imprimante par défaut dans Microsoft Edge qui doit être effectuée la première fois qu'un utilisateur essaie d’imprimer une page.

	Lorsque cette stratégie est définie, Microsoft Edge tente de trouver une imprimante qui correspond à tous les attributs spécifiés et l’utilise comme imprimante par défaut. Si plusieurs imprimantes remplissent les critères, la première imprimante correspondante est utilisée.

	Si vous ne configurez pas cette stratégie ou si aucune imprimante correspondante n'est détectée dans le délai imparti, l’imprimante est définie par défaut sur l’imprimante PDF intégrée ou sur aucune imprimante si l’imprimante PDF n’est pas disponible.

	La valeur est analysée en tant qu’objet JSON, conformément au schéma suivant : { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

	L'omission d'un champ signifie que toutes les valeurs correspondent ; par exemple, si vous ne spécifiez pas la connectivité, l'Aperçu avant impression démarre la découverte de tous les types d’imprimantes locales. Les modèles d’expressions régulières doivent respecter la syntaxe JavaScript RegExp et les correspondances respectent la casse.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultPrinterSelection
  - Nom de la stratégie de groupe: Règles de sélection d’imprimante par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Impression
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultPrinterSelection
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultPrinterSelection
  - Exemple de valeur :
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PrintHeaderFooter
  #### Imprimer des en-têtes et des pieds de page
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Forcez l'activation ou la désactivation des « en-têtes et pieds de page » dans la boîte de dialogue d’impression.

Si vous ne configurez pas cette stratégie, les utilisateurs peuvent décider d’imprimer les en-têtes et pieds de page.

Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas imprimer les en-têtes et pieds de page.

Si vous activez cette stratégie, les utilisateurs peuvent toujours imprimer les en-têtes et pieds de page.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PrintHeaderFooter
  - Nom de la stratégie de groupe: Imprimer des en-têtes et des pieds de page
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Impression
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Impression
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: PrintHeaderFooter
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PrintHeaderFooter
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PrintPreviewUseSystemDefaultPrinter
  #### Définir l’imprimante système par défaut en tant qu’imprimante par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Indique à Microsoft Edge d'utiliser l’imprimante système par défaut en tant qu’option par défaut dans l’aperçu avant impression à la place de l’imprimante la plus récemment utilisée.

	Si vous désactivez cette stratégie ou si vous ne la configurez pas, l'aperçu avant impression utilise l’imprimante la plus récemment utilisée comme option de destination par défaut.

	Si vous activez cette stratégie, l'aperçu avant impression utilise l’imprimante par défaut du système d’exploitation comme option de destination par défaut.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PrintPreviewUseSystemDefaultPrinter
  - Nom de la stratégie de groupe: Définir l’imprimante système par défaut en tant qu’imprimante par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Impression
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Impression
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: PrintPreviewUseSystemDefaultPrinter
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PrintPreviewUseSystemDefaultPrinter
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PrintingEnabled
  #### Activer l’impression
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active l’impression dans Microsoft Edge et empêche les utilisateurs de modifier ce paramètre.

	Si vous activez cette stratégie ou ne la configurez pas, les utilisateurs peuvent imprimer.

	Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas imprimer à partir de Microsoft Edge. L’impression est désactivée dans le menu clé, les extensions, les applications JavaScript, etc. Les utilisateurs peuvent toujours imprimer à partir de plug-ins qui n’utilisent pas Microsoft Edge lors de l’impression. Par exemple, certaines applications Adobe Flash présentent l'option d’impression dans leur menu contextuel, ce qui n’est pas couvert par cette stratégie.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PrintingEnabled
  - Nom de la stratégie de groupe: Activer l’impression
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Impression
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: PrintingEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PrintingEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### UseSystemPrintDialog
  #### Imprimer à l’aide de la boîte de dialogue d’impression système
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Affiche la boîte de dialogue d’impression système au lieu de l’aperçu avant impression.

	Si vous activez cette stratégie, Microsoft Edge ouvre la boîte de dialogue d’impression système à la place de l’aperçu avant impression intégré lorsque l’utilisateur imprime une page.

	Si vous ne configurez pas ou si vous désactivez cette stratégie, les commandes d’impression déclenchent l'écran Aperçu avant impression de Microsoft Edge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: UseSystemPrintDialog
  - Nom de la stratégie de groupe: Imprimer à l’aide de la boîte de dialogue d’impression système
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Impression
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: UseSystemPrintDialog
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: UseSystemPrintDialog
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Messagerie native policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### NativeMessagingAllowlist
  #### Contrôle des hôtes de messagerie natifs pouvant être utilisés par les utilisateurs
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  List specific native messaging hosts that users can use in Microsoft Edge.

By default, all native messaging hosts are allowed. If you set the [NativeMessagingBlocklist](#nativemessagingblocklist) policy to *, all native messaging hosts are blocked, and only native messaging hosts listed in here are loaded.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NativeMessagingAllowlist
  - Nom de la stratégie de groupe: Contrôle des hôtes de messagerie natifs pouvant être utilisés par les utilisateurs
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Messagerie native
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NativeMessagingAllowlist
  - Exemple de valeur :
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NativeMessagingBlocklist
  #### Configurer la liste rouge de messagerie native
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie les hôtes de messagerie natifs qui ne doivent pas être utilisés.

	Utilisez « * » pour bloquer tous les hôtes de messagerie natifs, à moins qu'ils ne soient explicitement répertoriés dans la liste verte.

	Si vous ne configurez pas cette stratégie, Microsoft Edge chargera tous les hôtes de messagerie natifs installés.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NativeMessagingBlocklist
  - Nom de la stratégie de groupe: Configurer la liste rouge de messagerie native
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Messagerie native
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NativeMessagingBlocklist
  - Exemple de valeur :
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NativeMessagingUserLevelHosts
  #### Autoriser les hôtes de messagerie natifs au niveau de l’utilisateur (installés sans autorisation d’administrateur)
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet l’installation d’hôtes de messagerie natifs au niveau utilisateur.

	Si vous désactivez cette stratégie, Microsoft Edge utilisera uniquement les hôtes de messagerie natifs installés au niveau système.

	Par défaut, si vous ne configurez pas cette stratégie, Microsoft Edge autorisera l'utilisation des hôtes de messagerie natifs au niveau utilisateur.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NativeMessagingUserLevelHosts
  - Nom de la stratégie de groupe: Autoriser les hôtes de messagerie natifs au niveau de l’utilisateur (installés sans autorisation d’administrateur)
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Messagerie native
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: NativeMessagingUserLevelHosts
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NativeMessagingUserLevelHosts
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Moteur de recherche par défaut policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderEnabled
  #### Activer le moteur de recherche par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active l’utilisation d’un moteur de recherche par défaut.

Si vous activez cette stratégie, un utilisateur peut rechercher un terme en tapant dans la barre d'adresse (tant que ce qu'il tape n’est pas une URL).

Vous pouvez spécifier le moteur de recherche par défaut à utiliser en activant le reste des stratégies de recherche par défaut. Si elles restent vides (non configurées), l’utilisateur peut choisir le moteur par défaut.

Si vous désactivez cette stratégie, l’utilisateur ne peut pas rechercher à partir de la barre d'adresse.

Si vous activez ou désactivez cette stratégie, les utilisateurs ne peuvent pas la modifier ni la remplacer.

Si vous ne configurez pas cette stratégie, le moteur de recherche par défaut est activé, et l’utilisateur peut choisir le moteur de recherche par défaut et définir la liste des moteurs de recherche.

Cette stratégie est disponible uniquement sur les instances de Windows jointes à un domaine Microsoft Active Directory ou sur les instances de Windows 10 Professionnel ou Entreprise inscrites pour la gestion des appareils.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderEnabled
  - Nom de la stratégie de groupe: Activer le moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultSearchProviderEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderEncodings
  #### Encodages du moteur de recherche par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specify the character encodings supported by the search provider. Encodings are code page names like UTF-8, GB2312, and ISO-8859-1. They are tried in the order provided.

This policy is optional. If not configured, the default, UTF-8, is used.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderEncodings
  - Nom de la stratégie de groupe: Encodages du moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderEncodings
  - Exemple de valeur :
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderImageURL
  #### Spécifie la fonction de recherche-par-image pour le moteur de recherche par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specifies the URL to the search engine used for image search. Search requests are sent using the GET method.

This policy is optional. If you don't configure it, image search isn't available.

Specify Bing's Image Search URL as:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'.

Specify Google's Image Search URL as: '{google:baseURL}searchbyimage/upload'.

See [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) policy to finish configuring image search.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderImageURL
  - Nom de la stratégie de groupe: Spécifie la fonction de recherche-par-image pour le moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultSearchProviderImageURL
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderImageURL
  - Exemple de valeur :
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderImageURLPostParams
  #### Paramètres pour une URL d’image qui utilise POST
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  If you enable this policy, it specifies the parameters used when an image search that uses POST is performed. The policy consists of comma-separated name/value pairs. If a value is a template parameter, like {imageThumbnail} in the preceding example, it’s replaced with real image thumbnail data. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

Specify Bing's Image Search URL Post Params as:
'imageBin={google:imageThumbnailBase64}'.

Specify Google's Image Search URL Post Params as:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

If you don’t set this policy, image search requests are sent using the GET method.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderImageURLPostParams
  - Nom de la stratégie de groupe: Paramètres pour une URL d’image qui utilise POST
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultSearchProviderImageURLPostParams
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderImageURLPostParams
  - Exemple de valeur :
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderKeyword
  #### Mot clé du moteur de recherche par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specifies the keyword, which is the shortcut used in the Address Bar to trigger the search for this provider.

This policy is optional. If you don't configure it, no keyword activates the search provider.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderKeyword
  - Nom de la stratégie de groupe: Mot clé du moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultSearchProviderKeyword
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"mis"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderKeyword
  - Exemple de valeur :
``` xml
<string>mis</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderName
  #### Nom du moteur de recherche par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specifies the name of the default search provider.

If you enable this policy, you set the name of the default search provider.

If you don't enable this policy or if you leave it empty, the host name specified by the search URL is used.

'DefaultSearchProviderName' should be set to an organization-approved encrypted search provider that corresponds to the encrypted search provider set in DTBC-0008. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderName
  - Nom de la stratégie de groupe: Nom du moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultSearchProviderName
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"My Intranet Search"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderName
  - Exemple de valeur :
``` xml
<string>My Intranet Search</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderSearchURL
  #### URL de recherche du moteur de recherche par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specifies the URL of the search engine used for a default search. The URL contains the string '{searchTerms}', which is replaced at query time by the terms the user is searching for.

Specify Bing's search URL as:

'{bing:baseURL}search?q={searchTerms}'.

Specify Google's search URL as: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

This policy is required when you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) policy; if you don't enable the latter policy, this policy is ignored.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderSearchURL
  - Nom de la stratégie de groupe: URL de recherche du moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultSearchProviderSearchURL
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderSearchURL
  - Exemple de valeur :
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultSearchProviderSuggestURL
  #### URL du moteur de recherche par défaut pour les suggestions
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specifies the URL for the search engine used to provide search suggestions. The URL contains the string '{searchTerms}', which is replaced at query time by the text the user has entered so far.

This policy is optional. If you don't configure it, users won't see search suggestions; they will see suggestions from their browsing history and favorites.

Bing's suggest URL can be specified as:

'{bing:baseURL}qbox?query={searchTerms}'.

Google's suggest URL can be specified as: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultSearchProviderSuggestURL
  - Nom de la stratégie de groupe: URL du moteur de recherche par défaut pour les suggestions
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Moteur de recherche par défaut
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultSearchProviderSuggestURL
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultSearchProviderSuggestURL
  - Exemple de valeur :
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Paramètres de SmartScreen policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### PreventSmartScreenPromptOverride
  #### Empêcher le contournement des avertissements de Microsoft Defender SmartScreen pour les sites
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  This policy setting lets you decide whether users can override the Microsoft Defender SmartScreen warnings about potentially malicious websites.

If you enable this setting, users can't ignore Microsoft Defender SmartScreen warnings and they are blocked from continuing to the site.

If you disable or don't configure this setting, users can ignore Microsoft Defender SmartScreen warnings and continue to the site.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PreventSmartScreenPromptOverride
  - Nom de la stratégie de groupe: Empêcher le contournement des avertissements de Microsoft Defender SmartScreen pour les sites
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de SmartScreen
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: PreventSmartScreenPromptOverride
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PreventSmartScreenPromptOverride
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PreventSmartScreenPromptOverrideForFiles
  #### Empêcher le contournement des avertissements de Microsoft Defender SmartScreen concernant les téléchargements
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure et sur Mac depuis la version 79 ou ultérieure

  #### Description
  This policy lets you determine whether users can override Microsoft Defender SmartScreen warnings about unverified downloads.

If you enable this policy, users in your organization can't ignore Microsoft Defender SmartScreen warnings, and they're prevented from completing the unverified downloads.

If you disable or don't configure this policy, users can ignore Microsoft Defender SmartScreen warnings and complete unverified downloads.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PreventSmartScreenPromptOverrideForFiles
  - Nom de la stratégie de groupe: Empêcher le contournement des avertissements de Microsoft Defender SmartScreen concernant les téléchargements
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de SmartScreen
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: PreventSmartScreenPromptOverrideForFiles
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PreventSmartScreenPromptOverrideForFiles
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SmartScreenAllowListDomains
  #### Configurer la liste des domaines pour lesquels Microsoft Defender SmartScreen ne déclenche pas d'avertissement
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configure the list of Microsoft Defender SmartScreen trusted domains. This means:
Microsoft Defender SmartScreen won't check for potentially malicious resources like phishing software and other malware if the source URLs match these domains.
The Microsoft Defender SmartScreen download protection service won't check downloads hosted on these domains.

If you enable this policy, Microsoft Defender SmartScreen trusts these domains.
If you disable or don't set this policy, default Microsoft Defender SmartScreen protection is applied to all resources.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.
Also note that this policy does not apply if your organization has enabled Microsoft Defender Advanced Threat Protection. You must configure your allow and block lists in Microsoft Defender Security Center instead.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SmartScreenAllowListDomains
  - Nom de la stratégie de groupe: Configurer la liste des domaines pour lesquels Microsoft Defender SmartScreen ne déclenche pas d'avertissement
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de SmartScreen
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SmartScreenAllowListDomains
  - Exemple de valeur :
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SmartScreenEnabled
  #### Configurer Microsoft Defender SmartScreen
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  This policy setting lets you configure whether to turn on Microsoft Defender SmartScreen. Microsoft Defender SmartScreen provides warning messages to help protect your users from potential phishing scams and malicious software. By default, Microsoft Defender SmartScreen is turned on.

If you enable this setting, Microsoft Defender SmartScreen is turned on.

If you disable this setting, Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SmartScreenEnabled
  - Nom de la stratégie de groupe: Configurer Microsoft Defender SmartScreen
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de SmartScreen
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Paramètres de SmartScreen
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: SmartScreenEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SmartScreenEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SmartScreenForTrustedDownloadsEnabled
  #### Forcer les vérifications de Microsoft Defender SmartScreen sur les téléchargements provenant de sources approuvées
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Cette stratégie vous permet de configurer la vérification par Microsoft Defender SmartScreen de la réputation des téléchargements à partir d'une source approuvée.

	Si vous activez ou ne configurez pas cette stratégie, Microsoft Defender SmartScreen vérifie la réputation des téléchargements, quelle qu'en soit la source.

	Si vous désactivez cette stratégie, Microsoft Defender SmartScreen ne vérifie pas la réputation des téléchargements lors d'un téléchargement à partir d'une source approuvée.

	Cette stratégie n’est disponible que sur les instances Windows qui sont jointes à un domaine Microsoft Active Directory ; ou sur des instances Windows 10 Professionnel ou Entreprise qui sont inscrites pour la gestion des appareils.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SmartScreenForTrustedDownloadsEnabled
  - Nom de la stratégie de groupe: Forcer les vérifications de Microsoft Defender SmartScreen sur les téléchargements provenant de sources approuvées
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de SmartScreen
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Paramètres de SmartScreen
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: SmartScreenForTrustedDownloadsEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SmartScreenPuaEnabled
  #### Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 80 ou ultérieure

  #### Description
  This policy setting lets you configure whether to turn on blocking for potentially unwanted apps in Microsoft Defender SmartScreen. Potentially unwanted app blocking in Microsoft Defender SmartScreen provides warning messages to help protect users from adware, coin miners, bundleware, and other low-reputation apps that are hosted by websites. Potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off by default.

If you enable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned on.

If you disable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use potentially unwanted app blocking in Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SmartScreenPuaEnabled
  - Nom de la stratégie de groupe: Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de SmartScreen
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Paramètres de SmartScreen
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: SmartScreenPuaEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SmartScreenPuaEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Paramètres de contenu policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### AutoSelectCertificateForUrls
  #### Sélectionner automatiquement des certificats clients pour ces sites
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specify a list of sites, based on URL patterns, for which Microsoft Edge should automatically select a client certificate, if the site requests one.

The value must be an array of stringified JSON dictionaries. Each dictionary must have the form { "pattern": "$URL_PATTERN", "filter" : $FILTER }, where $URL_PATTERN is a content setting pattern. $FILTER restricts from which client certificates the browser will automatically select. Independent of the filter, only certificates will be selected that match the server's certificate request. For example, if $FILTER has the form { "ISSUER": { "CN": "$ISSUER_CN" } }, additionally only client certificates are selected that are issued by a certificate with the CommonName $ISSUER_CN. If $FILTER contains an "ISSUER" and a "SUBJECT" section, a client certificate must satisfy both conditions to be selected. If $FILTER specifies an organization ("O"), a certificate must have at least one organization which matches the specified value to be selected. If $FILTER specifies an organization unit ("OU"), a certificate must have at least one organization unit which matches the specified value to be selected. If $FILTER is the empty dictionary {}, the selection of client certificates is not additionally restricted.

If you don't configure this policy, auto-selection isn't done for any site.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AutoSelectCertificateForUrls
  - Nom de la stratégie de groupe: Sélectionner automatiquement des certificats clients pour ces sites
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AutoSelectCertificateForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CookiesAllowedForUrls
  #### Autoriser les cookies sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that are allowed to set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesBlockedForUrls](#cookiesblockedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CookiesAllowedForUrls
  - Nom de la stratégie de groupe: Autoriser les cookies sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CookiesAllowedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CookiesBlockedForUrls
  #### Bloquer les cookies sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that can't set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CookiesBlockedForUrls
  - Nom de la stratégie de groupe: Bloquer les cookies sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CookiesBlockedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CookiesSessionOnlyForUrls
  #### Limiter les cookies provenant de sites web spécifiques à la session active
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Cookies created by websites that match a URL pattern you define are deleted when the session ends (when the window closes).

Cookies created by websites that don't match the pattern are controlled by the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or by the user's personal configuration. This is also the default behavior if you don't configure this policy.

If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See the [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

You can also use the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesBlockedForUrls](#cookiesblockedforurls) policies to control which websites can create cookies.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

If you set the [RestoreOnStartup](#restoreonstartup) policy to restore URLs from previous sessions, this policy is ignored, and cookies are stored permanently for those sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CookiesSessionOnlyForUrls
  - Nom de la stratégie de groupe: Limiter les cookies provenant de sites web spécifiques à la session active
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CookiesSessionOnlyForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultCookiesSetting
  #### Configurer les cookies
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Control whether websites can create cookies on the user's device. This policy is all or nothing - you can let all websites create cookies, or no websites create cookies. You can't use this policy to enable cookies from specific websites.

Set the policy to 'SessionOnly' (4) to clear cookies when the session closes. If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

If you don't configure this policy, the default 'AllowCookies' (1) is used, and users can change this setting in Microsoft Edge Settings. (If you don't want users to be able to change this setting, set the policy.)

* 1 = Let all sites create cookies

* 2 = Don't let any site create cookies

* 4 = Keep cookies for the duration of the session

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultCookiesSetting
  - Nom de la stratégie de groupe: Configurer les cookies
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultCookiesSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultCookiesSetting
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultGeolocationSetting
  #### Paramètre de géolocalisation par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Définissez si les sites web peuvent suivre les emplacements physiques des utilisateurs. Vous pouvez autoriser le suivi par défaut (1), le refuser par défaut (2) ou demander à l’utilisateur chaque fois qu’un site web demande son emplacement (3).

Si vous ne configurez pas cette stratégie, la stratégie « AskGeolocation » est utilisée et l’utilisateur peut modifier ce comportement.

* 1 = Autoriser les sites à suivre l’emplacement physique des utilisateurs

* 2 = Ne pas autoriser un site à effectuer le suivi d’emplacement physique des utilisateurs

* 3 = Demander chaque fois qu’un site souhaite suivre d’emplacement physique des utilisateurs

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultGeolocationSetting
  - Nom de la stratégie de groupe: Paramètre de géolocalisation par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultGeolocationSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultGeolocationSetting
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultImagesSetting
  #### Paramètres des images par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Définissez si les sites web peuvent afficher des images. Vous pouvez autoriser les images sur tous les sites (1) ou les bloquer sur tous les sites (2).

Si vous ne configurez pas cette stratégie, les images sont autorisées par défaut et l’utilisateur peut modifier ce paramètre.

* 1 = Autoriser tous les sites à afficher toutes les images

* 2 = N'autoriser aucun site à afficher les images

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultImagesSetting
  - Nom de la stratégie de groupe: Paramètres des images par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultImagesSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultImagesSetting
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultJavaScriptSetting
  #### Paramètre par défaut de JavaScript
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Définissez si les sites web peuvent exécuter JavaScript. Vous pouvez l'autoriser pour tous les sites (1) ou le bloquer pour tous les sites (2).

Si vous ne configurez pas cette stratégie, tous les sites peuvent exécuter JavaScript par défaut et l’utilisateur peut modifier ce paramètre.

* 1 = Autoriser tous les sites à exécuter JavaScript

* 2 = Ne pas autoriser les sites à exécuter JavaScript

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultJavaScriptSetting
  - Nom de la stratégie de groupe: Paramètre par défaut de JavaScript
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultJavaScriptSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultJavaScriptSetting
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultNotificationsSetting
  #### Paramètres de notification par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Définissez si les sites web peuvent afficher les notifications de bureau. Vous pouvez les autoriser par défaut (1), les refuser par défaut (2) ou demander que l’utilisateur reçoive une demande chaque fois qu’un site web veut afficher une notification (3).

Si vous ne configurez pas cette stratégie, les notifications sont autorisées par défaut et l’utilisateur peut modifier ce paramètre.

* 1 = Autoriser les sites à afficher les notifications du bureau

* 2 = Ne pas autoriser un site à afficher les notifications du bureau

* 3 = Demander chaque fois qu’un site souhaite afficher les notifications du bureau

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultNotificationsSetting
  - Nom de la stratégie de groupe: Paramètres de notification par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultNotificationsSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultNotificationsSetting
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultPluginsSetting
  #### Paramètre Adobe Flash par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Determines whether websites that aren't covered by [PluginsAllowedForUrls](#pluginsallowedforurls) or [PluginsBlockedForUrls](#pluginsblockedforurls) can automatically run the Adobe Flash plug-in. You can select 'BlockPlugins' (2) to block Adobe Flash on all sites, or you can select 'ClickToPlay' (3) to let Adobe Flash run but require the user to click the placeholder to start it. In any case, the [PluginsAllowedForUrls](#pluginsallowedforurls) and [PluginsBlockedForUrls](#pluginsblockedforurls) policies take precedence over 'DefaultPluginsSetting'.

Automatic playback is only allowed for domains explicitly listed in the [PluginsAllowedForUrls](#pluginsallowedforurls) policy. If you want to enable automatic playback for all sites, consider adding http://* and https://* to this list.

If you don't configure this policy, the user can change this setting manually.

* 2 = Block the Adobe Flash plug-in

* 3 = Click to play

The former '1' option set allow-all, but this functionality is now only handled by the [PluginsAllowedForUrls](#pluginsallowedforurls) policy.  Existing policies using '1' will operate in Click-to-play mode.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultPluginsSetting
  - Nom de la stratégie de groupe: Paramètre Adobe Flash par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultPluginsSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultPluginsSetting
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultPopupsSetting
  #### Paramètres de fenêtre contextuelle par défaut
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Définissez si les sites web peuvent afficher des fenêtres contextuelles. Vous pouvez les autoriser sur tous les sites web (1) ou les bloquer sur tous les sites (2).

Si vous ne configurez pas cette stratégie, des fenêtres contextuelles sont bloquées par défaut et les utilisateurs peuvent modifier ce paramètre.

* 1 = Autoriser tous les sites à afficher les fenêtres contextuelles

* 2 = Ne pas autoriser les sites à afficher les fenêtres contextuelles

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultPopupsSetting
  - Nom de la stratégie de groupe: Paramètres de fenêtre contextuelle par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultPopupsSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultPopupsSetting
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultWebBluetoothGuardSetting
  #### Contrôler l’utilisation de l’API web Bluetooth
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôler si les sites web peuvent accéder aux appareils Bluetooth à proximité. Vous pouvez complètement bloquer l’accès ou exiger que le site demande à l’utilisateur à chaque fois qu’il souhaite accéder à un appareil Bluetooth.

Si vous ne configurez pas cette stratégie, la valeur par défaut (3, qui signifie que les utilisateurs sont invités à chaque fois) est utilisée et les utilisateurs peuvent la modifier.

* 2 = N'autoriser aucun site à demander l’accès aux appareils Bluetooth en utilisant l’API web Bluetooth

* 3 = Autoriser les sites à demander à l’utilisateur d'accorder l’accès à un appareil Bluetooth à proximité

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultWebBluetoothGuardSetting
  - Nom de la stratégie de groupe: Contrôler l’utilisation de l’API web Bluetooth
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultWebBluetoothGuardSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultWebBluetoothGuardSetting
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultWebUsbGuardSetting
  #### Contrôler l’utilisation de l’API WebUSB
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Set whether websites can access connected USB devices. You can completely block access or ask the user each time a website wants to get access to connected USB devices.

You can override this policy for specific URL patterns by using the [WebUsbAskForUrls](#webusbaskforurls) and [WebUsbBlockedForUrls](#webusbblockedforurls) policies.

If you don't configure this policy, sites can ask users whether they can access the connected USB devices (3) by default, and users can change this setting.

* 2 = Don't allow any site to request access to USB devices via the WebUSB API

* 3 = Allow sites to ask the user to grant access to a connected USB device

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultWebUsbGuardSetting
  - Nom de la stratégie de groupe: Contrôler l’utilisation de l’API WebUSB
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultWebUsbGuardSetting
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultWebUsbGuardSetting
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImagesAllowedForUrls
  #### Autoriser les images sur ces sites
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that can display images.

If you don't configure this policy, the global default value is used for all sites either from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImagesAllowedForUrls
  - Nom de la stratégie de groupe: Autoriser les images sur ces sites
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImagesAllowedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImagesBlockedForUrls
  #### Bloquer les images sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that aren't allowed to display images.

If you don't configure this policy, the global default value from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImagesBlockedForUrls
  - Nom de la stratégie de groupe: Bloquer les images sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImagesBlockedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### JavaScriptAllowedForUrls
  #### Autoriser JavaScript sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that are allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: JavaScriptAllowedForUrls
  - Nom de la stratégie de groupe: Autoriser JavaScript sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: JavaScriptAllowedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### JavaScriptBlockedForUrls
  #### Bloquer JavaScript sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that aren't allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: JavaScriptBlockedForUrls
  - Nom de la stratégie de groupe: Bloquer JavaScript sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: JavaScriptBlockedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### LegacySameSiteCookieBehaviorEnabled
  #### Enable default legacy SameSite cookie behavior setting
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 80 ou ultérieure

  #### Description
  Lets you revert all cookies to legacy SameSite behavior. Reverting to legacy behavior causes cookies that don't specify a SameSite attribute to be treated as if they were "SameSite=None", and removes the requirement for "SameSite=None" cookies to carry the "Secure" attribute.

You can set the following values for this policy:

* 1 = Revert to legacy SameSite behavior for cookies on all sites

* 2 = Use SameSite-by-default behavior for cookies on all sites

If you don't set this policy, the default behavior for cookies that don't specify a SameSite attribute will depend on other configuration sources for the SameSite-by-default feature. This feature might be set by a field trial or by enabling the same-site-by-default-cookies flag in edge://flags.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: LegacySameSiteCookieBehaviorEnabled
  - Nom de la stratégie de groupe: Enable default legacy SameSite cookie behavior setting
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: LegacySameSiteCookieBehaviorEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: LegacySameSiteCookieBehaviorEnabled
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### LegacySameSiteCookieBehaviorEnabledForDomainList
  #### Revert to legacy SameSite behavior for cookies on specified sites
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 80 ou ultérieure

  #### Description
  Cookies set for domains match specified patterns will revert to legacy SameSite behavior.

Reverting to legacy behavior causes cookies that don't specify a SameSite attribute to be treated as if they were "SameSite=None", and removes the requirement for "SameSite=None" cookies to carry the "Secure" attribute.

If you don't set this policy, the global default value will be used. The global default will also be used for cookies on domains not covered by the patterns you specify.

The global default value can be configured using the [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) policy. If [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) is unset, the global default value falls back to other configuration sources.

Note that patterns you list in this policy are treated as domains, not URLs, so you should not specify a scheme or port.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Nom de la stratégie de groupe: Revert to legacy SameSite behavior for cookies on specified sites
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\0 = "www.example.com"
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\1 = "[*.]example.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Exemple de valeur :
``` xml
<array>
  <string>www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NotificationsAllowedForUrls
  #### Autoriser les notifications sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that can display notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NotificationsAllowedForUrls
  - Nom de la stratégie de groupe: Autoriser les notifications sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NotificationsAllowedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NotificationsBlockedForUrls
  #### Bloquer les notifications sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that are blocked from displaying notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NotificationsBlockedForUrls
  - Nom de la stratégie de groupe: Bloquer les notifications sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NotificationsBlockedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PluginsAllowedForUrls
  #### Autoriser le plug-in Adobe Flash sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that can run the Adobe Flash plug-in.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PluginsAllowedForUrls
  - Nom de la stratégie de groupe: Autoriser le plug-in Adobe Flash sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PluginsAllowedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PluginsBlockedForUrls
  #### Bloquer le plug-in Adobe Flash sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that are blocked from running Adobe Flash.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PluginsBlockedForUrls
  - Nom de la stratégie de groupe: Bloquer le plug-in Adobe Flash sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PluginsBlockedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PopupsAllowedForUrls
  #### Autoriser les fenêtres contextuelles sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that can open pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PopupsAllowedForUrls
  - Nom de la stratégie de groupe: Autoriser les fenêtres contextuelles sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PopupsAllowedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PopupsBlockedForUrls
  #### Bloquer les fenêtres contextuelles sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that are blocked from opening pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PopupsBlockedForUrls
  - Nom de la stratégie de groupe: Bloquer les fenêtres contextuelles sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PopupsBlockedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RegisteredProtocolHandlers
  #### Inscrire les gestionnaires de protocole
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Enregistrez une liste de gestionnaires de protocole. Définir la propriété de protocole sur le schéma (par exemple, « mailto ») et la propriété de l'URL sur le modèle d’URL de l’application qui gère le schéma. Le modèle peut inclure « %s », qui sera remplacé par l’URL traitée.

Vous pouvez recommander une valeur spécifique pour cette stratégie, mais vous ne pouvez pas exiger que vos utilisateurs l’utilisent.

Les gestionnaires de protocole enregistrés par la stratégie sont fusionnés avec les gestionnaires enregistrés par l’utilisateur et tous deux sont disponibles pour utilisation. L’utilisateur peut remplacer les gestionnaires de protocole installés par la stratégie en installant un nouveau gestionnaire par défaut, mais ils ne peuvent pas supprimer un gestionnaire de protocole enregistré par la stratégie.


  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Non
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RegisteredProtocolHandlers
  - Nom de la stratégie de groupe: Inscrire les gestionnaires de protocole
  - Chemin d'accès à la stratégie de groupe (Obligatoire): N/A
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/Paramètres de contenu
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): N/A
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: RegisteredProtocolHandlers
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: RegisteredProtocolHandlers
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### WebUsbAllowDevicesForUrls
  #### Accorder l’accès à des sites spécifiques pour se connecter à des périphériques USB spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Allows you to set a list of urls that specify which sites will automatically be granted permission to access a USB device with the given vendor and product IDs. Each item in the list must contain both devices and urls in order for the policy to be valid. Each item in devices can contain a vendor ID and product ID field. Any ID that is omitted is treated as a wildcard with one exception, and that exception is that a product ID cannot be specified without a vendor ID also being specified. Otherwise, the policy will not be valid and will be ignored.

The USB permission model uses the URL of the requesting site ("requesting URL") and the URL of the top-level frame site ("embedding URL") to grant permission to the requesting URL to access the USB device. The requesting URL may be different than the embedding URL when the requesting site is loaded in an iframe. Therefore, the "urls" field can contain up to two URL strings delimited by a comma to specify the requesting and embedding URL respectively. If only one URL is specified, then access to the corresponding USB devices will be granted when the requesting site's URL matches this URL regardless of embedding status. The URLs in "urls" must be valid URLs, otherwise the policy will be ignored.

If this policy is left not set, the global default value will be used for all sites either from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy if it is set, or the user's personal configuration otherwise.

URL patterns in this policy should not clash with the ones configured via [WebUsbBlockedForUrls](#webusbblockedforurls). If there is a clash, this policy will take precedence over [WebUsbBlockedForUrls](#webusbblockedforurls) and [WebUsbAskForUrls](#webusbaskforurls).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: WebUsbAllowDevicesForUrls
  - Nom de la stratégie de groupe: Accorder l’accès à des sites spécifiques pour se connecter à des périphériques USB spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: WebUsbAllowDevicesForUrls
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
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


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: WebUsbAllowDevicesForUrls
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### WebUsbAskForUrls
  #### Autoriser WebUSB sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that can ask the user for access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

The URL patterns defined in this policy can't conflict with those configured in the [WebUsbBlockedForUrls](#webusbblockedforurls) policy - you can't both allow and block a URL.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: WebUsbAskForUrls
  - Nom de la stratégie de groupe: Autoriser WebUSB sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: WebUsbAskForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### WebUsbBlockedForUrls
  #### Bloquer WebUSB sur des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that can't ask the user to grant them access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

URL patterns in this policy can't conflict with those configured in the [WebUsbAskForUrls](#webusbaskforurls) policy. You can't both allow and block a URL.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: WebUsbBlockedForUrls
  - Nom de la stratégie de groupe: Bloquer WebUSB sur des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Paramètres de contenu
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: WebUsbBlockedForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Serveur proxy policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### ProxyBypassList
  #### Configurer les règles de contournement du proxy
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Defines a list of hosts for which Microsoft Edge bypasses any proxy.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can create a list of hosts for which Microsoft Edge doesn't use a proxy.

If you don't configure this policy, no list of hosts is created for which Microsoft Edge bypasses a proxy. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more detailed examples go to [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ProxyBypassList
  - Nom de la stratégie de groupe: Configurer les règles de contournement du proxy
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Serveur proxy
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ProxyBypassList
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ProxyBypassList
  - Exemple de valeur :
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ProxyMode
  #### Configurer les paramètres du serveur proxy
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
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

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ProxyMode
  - Nom de la stratégie de groupe: Configurer les paramètres du serveur proxy
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Serveur proxy
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ProxyMode
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"direct"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ProxyMode
  - Exemple de valeur :
``` xml
<string>direct</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ProxyPacUrl
  #### Définir l'URL du fichier .pac du proxy
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specifies the URL for a proxy auto-config (PAC) file.

This policy is applied only if you selected 'Use a .pac proxy script' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can specify the URL for a PAC file, which defines how the browser automatically chooses the appropriate proxy server for fetching a particular website.

If you disable or don't configure this policy, no PAC file is specified. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ProxyPacUrl
  - Nom de la stratégie de groupe: Définir l'URL du fichier .pac du proxy
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Serveur proxy
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ProxyPacUrl
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://internal.contoso.com/example.pac"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ProxyPacUrl
  - Exemple de valeur :
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ProxyServer
  #### Configurer l’adresse ou l’URL du serveur proxy
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specifies the URL of the proxy server.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, the proxy server configured by this policy will be used for all URLs.

If you disable or don't configure this policy, users can choose their own proxy settings while in this proxy mode. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more options and detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ProxyServer
  - Nom de la stratégie de groupe: Configurer l’adresse ou l’URL du serveur proxy
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Serveur proxy
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ProxyServer
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"123.123.123.123:8080"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ProxyServer
  - Exemple de valeur :
``` xml
<string>123.123.123.123:8080</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ProxySettings
  #### Paramètres du proxy
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
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

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ProxySettings
  - Nom de la stratégie de groupe: Paramètres du proxy
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/Serveur proxy
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ProxySettings
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ProxySettings
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ## Additional policies

  [Revenir au début](#microsoft-edge---stratégies)

  ### AdsSettingForIntrusiveAdsSites
  #### Paramètres des annonces pour les sites contenant des annonces gênantes
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Contrôle si les annonces sont bloquées sur les sites contenant des annonces gênantes. Vous pouvez définir cette stratégie avec l'une des options suivantes :

	* 1 = Autorise les annonces sur tous les sites

	* 2 = Bloque les publicités sur les sites contenant des annonces gênantes (valeur par défaut).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AdsSettingForIntrusiveAdsSites
  - Nom de la stratégie de groupe: Paramètres des annonces pour les sites contenant des annonces gênantes
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AdsSettingForIntrusiveAdsSites
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AdsSettingForIntrusiveAdsSites
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AllowDeletingBrowserHistory
  #### Activer la suppression de l'historique du navigateur et des téléchargements
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet de supprimer l’historique du navigateur et l'historique de téléchargement, et empêche les utilisateurs de modifier ce paramètre.

	Notez que même si cette stratégie est désactivée, il n'est pas garanti que l’historique de navigation et de téléchargement sont conservés : les utilisateurs peuvent modifier ou supprimer directement les fichiers de base de données de l’historique et le navigateur proprement dit peut supprimer (en se basant sur la période d’expiration) ou archiver tout ou partie des éléments de l’historique à tout moment.

	Si vous activez cette stratégie ou si vous ne la configurez pas, les utilisateurs peuvent supprimer l’historique de navigation et de téléchargement.

	Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas supprimer l'historique de navigation et de téléchargement.

Si vous activez cette stratégie, n’activez pas la stratégie « Effacer les données de navigation à la fermeture de Microsoft Edge », car toutes deux concernent la suppression de données. Si vous les activez toutes les deux, la stratégie « Effacer les données de navigation à la fermeture de Microsoft Edge » est prioritaire et supprime toutes les données à la fermeture de Microsoft Edge, quelle que soit la configuration de cette stratégie.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AllowDeletingBrowserHistory
  - Nom de la stratégie de groupe: Activer la suppression de l'historique du navigateur et des téléchargements
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AllowDeletingBrowserHistory
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AllowDeletingBrowserHistory
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AllowFileSelectionDialogs
  #### Boîtes de dialogue Autoriser la sélection de fichiers
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Autoriser l’accès aux fichiers locaux en autorisant Microsoft Edge à afficher les boîtes de dialogue de sélection de fichier.

	Si vous activez ou ne configurez pas cette stratégie, les utilisateurs peuvent ouvrir des boîtes de dialogue de sélection de fichier comme d’habitude.

	Si vous désactivez cette stratégie, chaque fois que l’utilisateur effectue une action qui déclenche une boîte de dialogue de sélection de fichier (par exemple, l’importation des favoris, le téléchargement de fichiers ou l’enregistrement de liens), un message s’affiche et l’utilisateur est supposé avoir cliqué sur Annuler dans la boîte de dialogue de sélection de fichier.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AllowFileSelectionDialogs
  - Nom de la stratégie de groupe: Boîtes de dialogue Autoriser la sélection de fichiers
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AllowFileSelectionDialogs
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AllowFileSelectionDialogs
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AllowPopupsDuringPageUnload
  #### Autorise une page à afficher les fenêtres contextuelles pendant son déchargement
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Cette stratégie permet à un administrateur de spécifier qu’une page peut afficher des fenêtres contextuelles pendant le déchargement.

Lorsque la stratégie est activée, les pages sont autorisées à afficher des fenêtres contextuelles pendant leur déchargement.

Lorsque la stratégie est définie sur désactivé ou non défini, les pages ne sont pas autorisées à afficher des fenêtres contextuelles pendant leur déchargement. Ceci est conforme à la spécification : (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name).

Cette stratégie sera supprimée à l'avenir.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AllowPopupsDuringPageUnload
  - Nom de la stratégie de groupe: Autorise une page à afficher les fenêtres contextuelles pendant son déchargement
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AllowPopupsDuringPageUnload
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AllowPopupsDuringPageUnload
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AllowSyncXHRInPageDismissal
  #### Autoriser les pages à envoyer des demandes XHR synchrones lors de l’opération de rejet de page
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Cette stratégie vous permet de spécifier qu’une page peut envoyer des demandes XHR synchrones lors du rejet de page.

Si vous activez cette stratégie, les pages peuvent envoyer des demandes XHR synchrones lors du rejet de page.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, les pages ne sont pas autorisées à envoyer des demandes XHR synchrones lors du rejet de page.

Cette stratégie est temporaire et sera supprimée dans une version ultérieure.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AllowSyncXHRInPageDismissal
  - Nom de la stratégie de groupe: Autoriser les pages à envoyer des demandes XHR synchrones lors de l’opération de rejet de page
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AllowSyncXHRInPageDismissal
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AllowSyncXHRInPageDismissal
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AllowTrackingForUrls
  #### Configurer les exceptions de prévention du suivi pour des sites spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Configurez la liste des modèles d'URL qui sont exclus de la prévention du suivi.

	Si vous configurez cette stratégie, la liste des modèles d'URL configurés est exclue de la prévention du suivi.

	Si vous ne configurez pas cette stratégie, la valeur globale par défaut provenant de la stratégie « Bloquer le suivi des activités de navigation des utilisateurs » (si définie) ou la configuration personnelle de l'utilisateur est utilisée pour tous les sites.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AllowTrackingForUrls
  - Nom de la stratégie de groupe: Configurer les exceptions de prévention du suivi pour des sites spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AllowTrackingForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AlwaysOpenPdfExternally
  #### Toujours ouvrir les fichiers PDF en externe
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Désactive la visionneuse PDF interne dans Microsoft Edge.

	Si vous activez cette stratégie, Microsoft Edge traite les fichiers PDF comme des téléchargements et permet aux utilisateurs de les ouvrir avec l’application par défaut.

	Si vous ne configurez cette stratégie ou si vous la désactivez, Microsoft Edge ouvre les fichiers PDF (sauf si l’utilisateur désactive cette stratégie).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AlwaysOpenPdfExternally
  - Nom de la stratégie de groupe: Toujours ouvrir les fichiers PDF en externe
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AlwaysOpenPdfExternally
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AlwaysOpenPdfExternally
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ApplicationLocaleValue
  #### Définir les paramètres régionaux de l'application
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure

  #### Description
  Configure les paramètres régionaux de l'application dans Microsoft Edge et empêche les utilisateurs de modifier les paramètres régionaux.

	Si vous activez cette stratégie, Microsoft Edge utilise les paramètres régionaux spécifiés. Si le paramètre régional configuré n’est pas pris en charge, « en-US » est utilisé à la place.

	Si vous désactivez ou ne configurez pas ce paramètre, Microsoft Edge utilise les paramètres régionaux par défaut spécifiés par l’utilisateur (si configurés) ou le paramètre régional « en-US » de secours.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ApplicationLocaleValue
  - Nom de la stratégie de groupe: Définir les paramètres régionaux de l'application
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ApplicationLocaleValue
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"en"
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AudioCaptureAllowed
  #### Autoriser ou bloquer la capture audio
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Allows you to set whether a user is prompted to grant a website access to their audio capture device. This policy applies to all URLs except for those configured in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list.

If you enable this policy or don't configure it (the default setting), the user is prompted for audio capture access except from the URLs in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list. These listed URLs are granted access without prompting.

If you disable this policy, the user is not prompted, and audio capture is accessible only to the URLs configured in [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

This policy affects all types of audio inputs, not only the built-in microphone.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AudioCaptureAllowed
  - Nom de la stratégie de groupe: Autoriser ou bloquer la capture audio
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AudioCaptureAllowed
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AudioCaptureAllowed
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AudioCaptureAllowedUrls
  #### Sites pouvant accéder aux appareils de capture audio sans demander l’autorisation
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifiez les sites web, en fonction de modèles d’URL, qui peuvent utiliser des appareils de capture audio sans demander l’autorisation de l'utilisateur. Les modèles de cette liste sont comparés à l’origine de sécurité de l’URL d'incorporation. S'ils correspondent, le site reçoit automatiquement l’accès à des appareils de capture audio.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AudioCaptureAllowedUrls
  - Nom de la stratégie de groupe: Sites pouvant accéder aux appareils de capture audio sans demander l’autorisation
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AudioCaptureAllowedUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AutoImportAtFirstRun
  #### Importer automatiquement les données et les paramètres d’un autre navigateur lors de la première exécution
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Si vous activez cette stratégie, Microsoft Edge importe automatiquement tous les types de données et tous les paramètres pris en charge à partir du navigateur par défaut ou d’un autre navigateur spécifié. Cela force également Microsoft Edge à ignorer la section d’importation de l'expérience de première exécution.

	Si vous définissez cette stratégie sur « DisabledAutoImport » (4), la section d'importation de l’expérience de première exécution est totalement ignorée et Microsoft Edge n’importe pas automatiquement les données et les paramètres du navigateur.

	* 0 = Importe automatiquement tous les types de données et les paramètres pris en charge à partir du navigateur par défaut

	* 1 = Importe automatiquement tous les types de données et les paramètres pris en charge à partir d’Internet Explorer

	* 2 = Importe automatiquement tous les types de données et les paramètres pris en charge à partir de Google Chrome

	* 3 = Importe automatiquement tous les types de données et les paramètres pris en charge à partir de Safari

	* 4 = Désactive l’importation automatique et la section d'importation de l’expérience de première exécution est ignorée

	**Remarque** : cette stratégie prend actuellement en charge l’importation à partir d’Internet Explorer (sous Windows 7, 8 et 10), Google Chrome (sous Windows 7, 8 et 10 et sous macOS) et des navigateurs Apple Safari (sous macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AutoImportAtFirstRun
  - Nom de la stratégie de groupe: Importer automatiquement les données et les paramètres d’un autre navigateur lors de la première exécution
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AutoImportAtFirstRun
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AutoImportAtFirstRun
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AutofillAddressEnabled
  #### Activer le remplissage auto pour les adresses
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active la fonctionnalité Remplissage auto et permet aux utilisateurs de remplir automatiquement les informations d'adresse dans les formulaires web en utilisant les informations stockées précédemment.

	Si vous désactivez cette stratégie, la fonctionnalité Remplissage auto ne suggère jamais ni ne renseigne les informations d’adresse, et n’enregistre pas les informations d’adresse supplémentaires que l’utilisateur peut envoyer lors de la navigation sur le web.

	Si vous activez cette stratégie ou ne la configurez pas, les utilisateurs contrôlent le Remplissage auto pour les adresses dans l’interface utilisateur.

	Notez que si vous désactivez cette stratégie, vous arrêtez également toutes les activités pour tous les formulaires web, à l’exception des formulaires de paiement et de mot de passe. Aucune entrée supplémentaire n’est enregistrée et Microsoft Edge ne suggère pas ou ne remplit pas automatiquement les entrées précédentes.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AutofillAddressEnabled
  - Nom de la stratégie de groupe: Activer le remplissage auto pour les adresses
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: AutofillAddressEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AutofillAddressEnabled
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AutofillCreditCardEnabled
  #### Activer le Remplissage auto pour les cartes de crédit
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active la fonctionnalité Remplissage auto de Microsoft Edge et permet aux utilisateurs d'utiliser la saisie automatique pour les informations de carte de crédit dans les formulaires web en utilisant les informations stockées précédemment.

	Si vous désactivez cette stratégie, la fonctionnalité Remplissage auto ne suggère jamais ou ne remplit jamais les informations de carte de crédit, et n'enregistre pas les informations de carte de crédit supplémentaires que les utilisateurs peuvent envoyer lors de la navigation sur le web.

	Si vous activez cette stratégie ou ne la configurez pas, les utilisateurs contrôlent la fonctionnalité Remplissage auto pour les cartes de crédit.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AutofillCreditCardEnabled
  - Nom de la stratégie de groupe: Activer le Remplissage auto pour les cartes de crédit
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: AutofillCreditCardEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AutofillCreditCardEnabled
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### AutoplayAllowed
  #### Autoriser la lecture automatique de média pour les sites web
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Cette stratégie définit la stratégie de lecture automatique de médias pour les sites web.

Le paramètre par défaut, « Non configuré », respecte les paramètres actuels de lecture automatique de médias et permet aux utilisateurs de configurer leurs paramètres de lecture automatique.

Le paramètre « Activé » définit la lecture automatique de médias sur « Autoriser ». Tous les sites web sont autorisés à lire les médias par lecture automatique. Les utilisateurs ne peuvent pas remplacer cette stratégie.

Le paramètre « Désactivé » définit la lecture automatique de médias sur « Bloquer ». Aucun site web n’est autorisé à procéder à la lecture automatique des médias. Les utilisateurs ne peuvent pas remplacer cette stratégie.

Un onglet doit être fermé et rouvert pour que cette stratégie prenne effet.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: AutoplayAllowed
  - Nom de la stratégie de groupe: Autoriser la lecture automatique de média pour les sites web
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: AutoplayAllowed
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: AutoplayAllowed
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BackgroundModeEnabled
  #### Poursuivre l’exécution des applications en arrière-plan après la fermeture de Microsoft Edge
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure

  #### Description
  Permet aux processus de Microsoft Edge de démarrer lors de la connexion du système d’exploitation et de continuer à s’exécuter après la fermeture de la dernière fenêtre du navigateur. Dans ce scénario, les applications en arrière-plan et la session de navigation actuelle restent actives, y compris les cookies de la session. Un processus ouvert en arrière-plan affiche une icône dans la barre d’état système et peut toujours être fermé à partir de cet emplacement.

	Si vous activez cette stratégie, le mode arrière-plan est activé.

	Si vous désactivez cette stratégie, le mode arrière-plan est désactivé.

	Si vous ne configurez pas cette stratégie, le mode arrière-plan est désactivé et l’utilisateur peut configurer son comportement dans edge://settings/system.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BackgroundModeEnabled
  - Nom de la stratégie de groupe: Poursuivre l’exécution des applications en arrière-plan après la fermeture de Microsoft Edge
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: BackgroundModeEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BackgroundTemplateListUpdatesEnabled
  #### Active les mises à jour en arrière-plan dans la liste des modèles disponibles pour les collections et d’autres fonctionnalités qui utilisent des modèles.
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Vous permet d’activer ou de désactiver les mises à jour en arrière-plan pour la liste des modèles disponibles pour les collections et d’autres fonctionnalités qui utilisent des modèles. Les modèles permettent d'extraire des métadonnées enrichies d’une page web lorsque la page est enregistrée dans une collection.

Si vous activez ce paramètre ou si le paramètre n’est pas configuré, la liste des modèles disponibles est téléchargée en arrière-plan à partir d’un service Microsoft toutes les 24 heures.

Si vous désactivez ce paramètre, la liste des modèles disponibles est téléchargée à la demande. Ce type de téléchargement peut entraîner de légères altérations des performances pour les collections et d’autres fonctionnalités.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BackgroundTemplateListUpdatesEnabled
  - Nom de la stratégie de groupe: Active les mises à jour en arrière-plan dans la liste des modèles disponibles pour les collections et d’autres fonctionnalités qui utilisent des modèles.
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: BackgroundTemplateListUpdatesEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: BackgroundTemplateListUpdatesEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BlockThirdPartyCookies
  #### Bloquer les cookies tiers
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Empêcher les éléments de page web qui ne proviennent pas du domaine qui se trouve dans la barre d’adresses de définir des cookies.

Si vous activez cette stratégie, les éléments de page web qui ne proviennent pas du domaine qui se trouve dans la barre d’adresses ne peuvent pas définir de cookies

Si vous désactivez cette stratégie, les éléments de page web provenant de domaines autres que ceux figurant dans la barre d’adresses peuvent définir des cookies.

Si vous ne configurez pas cette stratégie, des cookies tiers sont activés, mais les utilisateurs peuvent modifier ce paramètre.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BlockThirdPartyCookies
  - Nom de la stratégie de groupe: Bloquer les cookies tiers
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: BlockThirdPartyCookies
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: BlockThirdPartyCookies
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BrowserAddProfileEnabled
  #### Activer la création de profil à partir du menu déroulant Identité ou de la page Paramètres
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Autorise les utilisateurs de créer des profils à l’aide de l’option **Ajouter un profil**.
	Si vous activez cette stratégie ou ne la configurez pas, Microsoft Edge autorise les utilisateurs à utiliser **Ajouter un profil** dans le menu déroulant Identité ou sur la page Paramètres pour créer des profils.

	Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas ajouter de profils à partir du menu déroulant Identité ou de la page Paramètres.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BrowserAddProfileEnabled
  - Nom de la stratégie de groupe: Activer la création de profil à partir du menu déroulant Identité ou de la page Paramètres
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: BrowserAddProfileEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: BrowserAddProfileEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BrowserGuestModeEnabled
  #### Activer le mode invité
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Activez l’option autorisant l’utilisation de profils invités dans Microsoft Edge. Dans un profil invité, le navigateur n’importe pas les données de navigation à partir des profils existants et supprime les données de navigation lorsque tous les profils invités sont fermés.

	Si vous activez cette stratégie ou ne la configurez pas, Microsoft Edge permet aux utilisateurs de parcourir les profils invités.

	Si vous désactivez cette stratégie, Microsoft Edge n’autorise pas les utilisateurs à parcourir les profils invités.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BrowserGuestModeEnabled
  - Nom de la stratégie de groupe: Activer le mode invité
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: BrowserGuestModeEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: BrowserGuestModeEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BrowserNetworkTimeQueriesEnabled
  #### Autoriser les requêtes auprès d'un service de temps réseau de navigateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Empêche Microsoft Edge de parfois envoyer des requêtes à un service de temps réseau du navigateur pour récupérer un horodatage précis.

	Si vous désactivez cette stratégie, Microsoft Edge arrête d’envoyer des requêtes à un service de temps réseau du navigateur.

	Si vous activez cette stratégie ou si vous ne la configurez pas, Microsoft Edge envoie parfois des requêtes à un service de temps réseau du navigateur.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BrowserNetworkTimeQueriesEnabled
  - Nom de la stratégie de groupe: Autoriser les requêtes auprès d'un service de temps réseau de navigateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: BrowserNetworkTimeQueriesEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: BrowserNetworkTimeQueriesEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BrowserSignin
  #### Paramètres de connexion du navigateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specify whether a user can sign into Microsoft Edge with their account and use account-related services like sync and single sign on. To control the availability of sync, use the [SyncDisabled](#syncdisabled) policy instead.

If you set this policy to 'Disable browser sign-in', make sure that you also set the [NonRemovableProfileEnabled](#nonremovableprofileenabled) policy to disabled because [NonRemovableProfileEnabled](#nonremovableprofileenabled) disables the creation of an automatically signed in browser profile. If both policies are set, Microsoft Edge will use the 'Disable browser sign-in' policy and behave as if [NonRemovableProfileEnabled](#nonremovableprofileenabled) is set to disabled.

If you set this policy to 'Enable browser sign-in' (1), users can sign into the browser. Signing into the browser doesn't mean that sync is turned on by default; the user must separately opt-in to use this feature.

If you set this policy to 'Force browser sign-in' (2) users must sign into a profile to use the browser. By default, this will allow the user to choose whether they want to sync to their account, unless sync is disabled by the domain admin or with the [SyncDisabled](#syncdisabled) policy. The default value of [BrowserGuestModeEnabled](#browserguestmodeenabled) policy is set to false.

If you don't configure this policy users can decide if they want to enable the browser sign-in option and use it as they see fit.

* 0 = Disable browser sign-in

* 1 = Enable browser sign-in

* 2 = Force users to sign-in to use the browser

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BrowserSignin
  - Nom de la stratégie de groupe: Paramètres de connexion du navigateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: BrowserSignin
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: BrowserSignin
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### BuiltInDnsClientEnabled
  #### Utiliser le client DNS intégré
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôle s’il convient d'utiliser le client DNS intégré.

Si vous activez cette stratégie, le client DNS intégré est utilisé s'il est disponible.

Si vous désactivez cette stratégie, le client n’est jamais utilisé.

Si vous ne configurez pas cette stratégie, le client DNS intégré est activé par défaut sur MacOS et les utilisateurs peuvent modifier s’il convient d'utiliser le client DNS intégré en modifiant edge://flags ou en spécifiant un indicateur de ligne de commande.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: BuiltInDnsClientEnabled
  - Nom de la stratégie de groupe: Utiliser le client DNS intégré
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: BuiltInDnsClientEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: BuiltInDnsClientEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### Désactiver l'application transparence de certificat pour la liste des hachages subjectPublicKeyInfo
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Désactive l’application des exigences de transparence du certificat pour obtenir la liste des hachages subjectPublicKeyInfo.

Cette stratégie vous permet de désactiver les exigences de divulgation de transparence de certificat pour les chaînes de certificat qui contiennent des certificats avec l’un des hachages subjectPublicKeyInfo spécifiés. Ceci autorise les certificats qui ne seraient pas approuvés dans le cas contraire, car ils n'ont pas été divulgués publiquement correctement, à continuer à être utilisés pour les hôtes Entreprise.

Pour désactiver l'application de la transparence du certificat lorsque cette stratégie est définie, l'un des ensembles de conditions suivants doit être rempli :
1. Le hachage est celui de subjectPublicKeyInfo du certificat serveur.
2. Le hachage est celui d’un subjectPublicKeyInfo qui s’affiche dans un certificat d’autorité de certification dans la chaîne de certificats, que le certificat d’autorité de certification est limité via l’extension nameConstraints X.509v3, au moins un nameConstraints est présent dans le permittedSubtrees et le directoryName contient un attribut organizationName.
3. Le hachage est celui d’un subjectPublicKeyInfo qui s’affiche dans un certificat d’autorité de certification dans la chaîne de certificats, que le certificat d’autorité de certification a au moins un attribut organizationName dans le sujet du certificat et le certificat du serveur contient le même nombre d'attributs organizationName, dans le même ordre et avec les valeurs identiques (octet pour octet).

Un hachage subjectPublicKeyInfo est spécifié par la concaténation du nom d’algorithme de hachage, le caractère « / » et l’encodage Base64 de cet algorithme de hachage appliqué à la subjectPublicKeyInfo codée DER du certificat spécifié. Cet encodage Base64 est le même format qu’une empreinte digitale SPKI, telle que définie dans la RFC 7469, section 2.4. Les algorithmes de hachage non reconnus sont ignorés. Le seul algorithme de hachage pris en charge pour l’instant est « sha256 ».

Si vous désactivez ou ne configurez pas cette stratégie, tous les certificats obligatoires pour être divulgués via la transparence des certificats sont considérés comme non approuvés s'ils ne sont pas transmis conformément à la stratégie de transparence du certificat.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CertificateTransparencyEnforcementDisabledForCas
  - Nom de la stratégie de groupe: Désactiver l'application transparence de certificat pour la liste des hachages subjectPublicKeyInfo
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CertificateTransparencyEnforcementDisabledForCas
  - Exemple de valeur :
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### Désactivez l’application de transparence de certificat pour obtenir la liste des autorités de certification héritées
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Désactive l’application des exigences de transparence de certificat pour une liste d’autorités de certification (AC) héritées.

	Cette stratégie vous permet de désactiver les exigences de divulgation de transparence de certificat pour les chaînes de certificat qui contiennent des certificats avec l’un des hachages subjectPublicKeyInfo spécifiés. Ainsi, les certificats qui ne seraient pas approuvés en temps normal, car ils n’ont pas été correctement divulgués publiquement, continuent à être utilisés pour les hôtes de l’entreprise.

	Pour pouvoir désactiver l'application de la transparence de certificat, vous devez définir le hachage sur un subjectPublicKeyInfo apparaissant dans un certificat d’autorité de certification qui n’est reconnu comme une autorité de certification (AC) héritée. Une autorité de certification héritée est une autorité de certification qui a été approuvée publiquement par défaut par un ou plusieurs systèmes d’exploitation pris en charge par Microsoft Edge.

	Pour spécifier un hachage subjectPublicKeyInfo, concaténez le nom de l’algorithme de hachage, le caractère « / » et l’encodage Base64 de cet algorithme de hachage appliqué à la subjectPublicKeyInfo codée DER du certificat spécifié. Cet encodage Base64 est le même format qu’une empreinte digitale SPKI, tel que défini dans RFC 7469, Section 2.4. Les algorithmes de hachage non reconnus sont ignorés. Le seul algorithme de hachage pris en charge pour l’instant est « sha256 ».

	Si vous ne configurez pas cette stratégie, tous les certificats qui doivent être divulgués via la transparence des certificats sont considérés comme non approuvés s'ils ne sont pas divulgués conformément à la stratégie de transparence de certificat.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Nom de la stratégie de groupe: Désactivez l’application de transparence de certificat pour obtenir la liste des autorités de certification héritées
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Exemple de valeur :
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### Désactiver l'application de transparence de certificat pour des URL spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Désactive l’application des exigences de transparence de certificat pour les URL répertoriées.

	Cette stratégie vous permet de ne pas divulguer les certificats pour les noms d’hôte dans les URL spécifiées via la transparence du certificat. Cela vous permet d’utiliser les certificats qui ne seraient pas approuvés, car ils n’ont pas été correctement publiés, mais elle complique la détection des certificats mal utilisés pour ces hôtes.

	Formez le modèle d’URL de la façon suivante : [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322). Étant donné que les certificats sont valides pour un nom d’hôte donné, indépendamment du schéma, port ou chemin d’accès, seule une partie du nom d’hôte de l’URL est prise en compte. Les hôtes de caractères génériques ne sont pas pris en charge.

	Si vous ne configurez pas cette stratégie, tous les certificats qui doivent être transmis via la transparence du certificat sont considérés comme non approuvés s’ils ne sont pas divulgués.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CertificateTransparencyEnforcementDisabledForUrls
  - Nom de la stratégie de groupe: Désactiver l'application de transparence de certificat pour des URL spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CertificateTransparencyEnforcementDisabledForUrls
  - Exemple de valeur :
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ClearBrowsingDataOnExit
  #### Effacer les données de navigation à la fermeture de Microsoft Edge
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Microsoft Edge doesn't clear the browsing data by default when it closes. Browsing data includes information entered in forms, passwords, and even the websites visited.

If you enable this policy, all browsing data is deleted each time Microsoft Edge closes.

If you disable or don't configure this policy, users can configure the Clear browsing data option in Settings.

If you enable this policy, don't enable the [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) policy, because they both deal with deleting data. If you enable both, this policy takes precedence and deletes all data when Microsoft Edge closes, regardless of how you configured [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ClearBrowsingDataOnExit
  - Nom de la stratégie de groupe: Effacer les données de navigation à la fermeture de Microsoft Edge
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ClearBrowsingDataOnExit
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ClearBrowsingDataOnExit
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ClickOnceEnabled
  #### Autoriser les utilisateurs à ouvrir des fichiers à l’aide du protocole ClickOnce
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Autoriser les utilisateurs à ouvrir des fichiers à l’aide du protocole ClickOnce. Le protocole ClickOnce permet aux sites web de demander que le navigateur ouvre les fichiers d’une URL spécifique à l’aide du gestionnaire de fichiers ClickOnce sur l’ordinateur ou l’appareil de l’utilisateur.

Si vous activez cette stratégie, les utilisateurs peuvent ouvrir des fichiers à l’aide du protocole ClickOnce. Cette stratégie remplace le paramètre ClickOnce de l’utilisateur sur la page edge://flags/.

Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas ouvrir de fichiers à l’aide du protocole ClickOnce. Au lieu de cela, le fichier est enregistré dans le système de fichiers utilisant le navigateur. Cette stratégie remplace le paramètre ClickOnce de l’utilisateur sur la page edge://flags/.

Si vous ne configurez pas cette stratégie, les utilisateurs ne peuvent pas ouvrir de fichiers à l’aide du protocole ClickOnce. Les utilisateurs ont la possibilité d’activer l’utilisation du protocole ClickOnce avec la page edge://flags/.

La désactivation de ClickOnce peut empêcher le lancement correct d’applications ClickOnce (fichiers .application).

Pour plus d’informations sur ClickOnce, voir [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) and [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ClickOnceEnabled
  - Nom de la stratégie de groupe: Autoriser les utilisateurs à ouvrir des fichiers à l’aide du protocole ClickOnce
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ClickOnceEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CommandLineFlagSecurityWarningsEnabled
  #### Activer les avertissements de sécurité pour les indicateurs de ligne de commande
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Si cette stratégie est désactivée, elle empêche l'apparition des avertissements de sécurité lorsque Microsoft Edge est lancé avec des indicateurs de ligne de commande potentiellement dangereux.

Si elle est activée ou non configurée, les avertissements de sécurité s'affichent lorsque ces indicateurs de ligne de commande sont utilisés pour lancer Microsoft Edge.

Par exemple, l'indicateur « --disable-gpu-sandbox » génère l'avertissement suivant :  Vous utilisez un indicateur de ligne de commande non pris en charge : « --disable-gpu-sandbox ». Cela implique des risques de sécurité et de stabilité.

Sur Windows, cette stratégie est uniquement disponible sur les instances jointes au domaine Microsoft Active Directory, ou sur Windows 10 Professionnel (ou Enterprise) sur les instances engagées dans la gestion d'un appareil.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CommandLineFlagSecurityWarningsEnabled
  - Nom de la stratégie de groupe: Activer les avertissements de sécurité pour les indicateurs de ligne de commande
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: CommandLineFlagSecurityWarningsEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CommandLineFlagSecurityWarningsEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ComponentUpdatesEnabled
  #### Activer les mises à jour de composant dans Microsoft Edge
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Si vous activez ou ne configurez pas cette stratégie, les mises à jour de composant sont activées dans Microsoft Edge.

	Si vous désactivez cette stratégie ou la définissez sur « false », les mises à jour de composant sont désactivées pour tous les composants dans Microsoft Edge.

	Toutefois, certains composants ne sont pas concernés par cette stratégie, notamment les composants ne contenant pas de code exécutable, ceux qui n'affectent pas de manière importante le comportement du navigateur ou encore ceux qui sont importants pour la sécurité. En d'autres termes, les mises à jour considérées comme « importante pour la sécurité » sont toujours appliquées même si vous désactivez la stratégie.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ComponentUpdatesEnabled
  - Nom de la stratégie de groupe: Activer les mises à jour de composant dans Microsoft Edge
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ComponentUpdatesEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ComponentUpdatesEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ConfigureDoNotTrack
  #### Configurer Ne pas me suivre
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifiez s’il faut envoyer des requêtes Ne pas me suivre aux sites web qui demandent des infos de suivi. Les requêtes Ne pas me suivre autorisent les sites web que vous visitez à savoir que vous ne souhaitez pas que votre activité de navigation soit suivie. Par défaut, Microsoft Edge n’envoie pas de requête Ne pas me suivre, mais les utilisateurs peuvent activer cette fonctionnalité pour les envoyer.

	Si vous activez cette stratégie, les requêtes Ne pas me suivre sont toujours envoyées aux sites web qui demandent des infos de suivi.

	Si vous désactivez cette stratégie, les requêtes ne sont jamais envoyées.

	Si vous ne configurez pas cette stratégie, les utilisateurs peuvent décider d’envoyer ces requêtes.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ConfigureDoNotTrack
  - Nom de la stratégie de groupe: Configurer Ne pas me suivre
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ConfigureDoNotTrack
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ConfigureDoNotTrack
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ConfigureOnlineTextToSpeech
  #### Configuration la conversion de texte par synthèse vocale en ligne
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Set whether the browser can leverage Online Text to Speech voice fonts, part of Azure Cognitive Services. These voice fonts are higher quality than the pre-installed system voice fonts.

If you enable or don't configure this policy, web-based applications that use the SpeechSynthesis API can use Online Text to Speech voice fonts.

If you disable this policy, the voice fonts aren't available.

Read more about this feature here:
SpeechSynthesis API: [https://go.microsoft.com/fwlink/?linkid=2110038](https://go.microsoft.com/fwlink/?linkid=2110038)
Cognitive Services: [https://go.microsoft.com/fwlink/?linkid=2110141](https://go.microsoft.com/fwlink/?linkid=2110141)

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ConfigureOnlineTextToSpeech
  - Nom de la stratégie de groupe: Configuration la conversion de texte par synthèse vocale en ligne
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ConfigureOnlineTextToSpeech
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ConfigureOnlineTextToSpeech
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### CustomHelpLink
  #### Spécifier le lien d’aide personnalisé
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Spécifiez un lien pour le menu d’aide ou la touche F1.

Si vous activez cette stratégie, un administrateur peut spécifier un lien pour le menu d’aide ou la touche F1.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, le lien par défaut du menu d'aide ou de la touche F1 est utilisé.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: CustomHelpLink
  - Nom de la stratégie de groupe: Spécifier le lien d’aide personnalisé
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: CustomHelpLink
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: CustomHelpLink
  - Exemple de valeur :
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DefaultBrowserSettingEnabled
  #### Définir Microsoft Edge comme navigateur par défaut
  >Versions prises en charge : Microsoft Edge sur Windows 7 et Mac depuis la version 77 ou ultérieure

  #### Description
  Configure les vérifications du navigateur par défaut dans Microsoft Edge et empêche les utilisateurs de les modifier.

	Si vous activez cette stratégie, Microsoft Edge vérifie toujours au démarrage s’il s’agit du navigateur par défaut et s’inscrit automatiquement, si possible.

	Si vous désactivez cette stratégie, Microsoft Edge n’effectue jamais de vérification et désactive les contrôles utilisateur pour définir cette option.

	Si vous ne configurez pas cette stratégie, Microsoft Edge permet à l’utilisateur de contrôler s’il s'agit du navigateur par défaut et d’afficher les notifications utilisateur lorsque ce n'est pas le cas.

	Remarque à l’attention des administrateurs Windows : cette stratégie ne fonctionne que pour les PC exécutant Windows 7. Pour les versions ultérieures de Windows, vous devez déployer un fichier « associations d’applications par défaut » qui fait de Microsoft Edge le gestionnaire pour les protocoles HTTPS et HTTP (et, éventuellement, le protocole FTP et les formats de fichier, tels que .html, .htm, .pdf, .svg, .webp). Voir [https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932) pour plus d’informations.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DefaultBrowserSettingEnabled
  - Nom de la stratégie de groupe: Définir Microsoft Edge comme navigateur par défaut
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DefaultBrowserSettingEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DefaultBrowserSettingEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DeveloperToolsAvailability
  #### Contrôler où les outils de développement peuvent être utilisés
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôler l’emplacement où les outils de développement peuvent être utilisés.

Si vous définissez cette stratégie sur « DeveloperToolsDisallowedForForceInstalledExtensions » (0, valeur par défaut), les utilisateurs peuvent accéder aux outils de développement et à la console JavaScript en général, mais pas dans le contexte des extensions installées par la stratégie d’entreprise.

Si vous définissez cette stratégie sur « DeveloperToolsAllowed » (1), les utilisateurs peuvent accéder aux outils de développement et à la console JavaScript dans tous les contextes, y compris les extensions installées par la stratégie d’entreprise.

Si vous définissez cette stratégie sur « DeveloperToolsDisallowed » (2), les utilisateurs ne peuvent pas accéder aux outils de développement ni inspecter les éléments du site web. Les raccourcis clavier et les entrées de menu ou de menu contextuel qui ouvrent les outils de développement ou la console JavaScript sont désactivées.

* 0 = Bloquer les outils de développement sur les extensions installées par la stratégie d’entreprise, autoriser dans les autres contextes

* 1 = Autoriser l'utilisation des outils de développement

* 2 = Ne pas autoriser l’utilisation des outils de développement

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DeveloperToolsAvailability
  - Nom de la stratégie de groupe: Contrôler où les outils de développement peuvent être utilisés
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DeveloperToolsAvailability
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DeveloperToolsAvailability
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DirectInvokeEnabled
  #### Autoriser les utilisateurs à ouvrir des fichiers à l’aide du protocole DirectInvoke
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Autorisez les utilisateurs à ouvrir des fichiers à l’aide du protocole DirectInvoke. Le protocole DirectInvoke permet aux sites web de demander que le navigateur ouvre les fichiers d’une URL spécifique à l’aide d’un gestionnaire de fichiers spécifique sur l’ordinateur ou l’appareil de l’utilisateur.

Si vous activez ou ne configurez pas cette stratégie, les utilisateurs peuvent ouvrir des fichiers à l’aide du protocole DirectInvoke.

Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas ouvrir de fichiers à l’aide du protocole DirectInvoke. Au lieu de cela, le fichier est enregistré dans le système de fichiers.

Remarque : la désactivation de DirectInvoke peut empêcher certaines fonctionnalités de Microsoft Office SharePoint Online de s’utiliser comme prévu.

Pour plus d’informations sur DirectInvoke, voir [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) et [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DirectInvokeEnabled
  - Nom de la stratégie de groupe: Autoriser les utilisateurs à ouvrir des fichiers à l’aide du protocole DirectInvoke
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DirectInvokeEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### Disable3DAPIs
  #### Désactiver la prise en charge des API graphiques 3D
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Prevent web pages from accessing the graphics processing unit (GPU). Specifically, web pages can't access the WebGL API and plug-ins can't use the Pepper 3D API.

If you don't configure or disable this policy, it potentially allows web pages to use the WebGL API and plug-ins to use the Pepper 3D API. Microsoft Edge might, by default, still require command line arguments to be passed in order to use these APIs.

If [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) policy is set to false, the setting for 'Disable3DAPIs' policy is ignored - it's the equivalent of setting 'Disable3DAPIs' policy to true.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: Disable3DAPIs
  - Nom de la stratégie de groupe: Désactiver la prise en charge des API graphiques 3D
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: Disable3DAPIs
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: Disable3DAPIs
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DisableScreenshots
  #### Désactiver la création de captures d’écran
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôle si les utilisateurs peuvent prendre des captures d’écran de la page du navigateur.

Si cette option est activée, l’utilisateur ne peut pas prendre de captures d’écran à l’aide des raccourcis clavier ou des API d’extension.

Si cette option est désactivée ou si vous ne configurez pas cette stratégie, les utilisateurs peuvent prendre des captures d’écran.

Veuillez noter que cette stratégie contrôle les captures d’écran prises dans le navigateur proprement dit. Même si vous activez cette stratégie, les utilisateurs peuvent toujours prendre des captures d’écran en utilisant une méthode en dehors du navigateur (comme l’utilisation d’une fonctionnalité du système d’exploitation ou d’une autre application).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DisableScreenshots
  - Nom de la stratégie de groupe: Désactiver la création de captures d’écran
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DisableScreenshots
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DisableScreenshots
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DiskCacheDir
  #### Définir le répertoire du cache du disque
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configure le répertoire à utiliser pour stocker les fichiers mis en cache.

	Si vous activez cette stratégie, Microsoft Edge utilise le répertoire spécifié, peu importe si l’utilisateur a spécifié l'indicateur « --disk-cache-dir ». Pour éviter toute perte de données ou d’autres erreurs inattendues, ne configurez pas cette stratégie au répertoire racine d’un volume ni dans un répertoire utilisé à d’autres fins, car Microsoft Edge gère son contenu.

	Voir [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) pour obtenir la liste des variables, que vous pouvez utiliser lorsque vous spécifiez les répertoires et les chemins d’accès.

	Si vous ne configurez pas ce paramètre de stratégie, le répertoire de cache par défaut est utilisé et les utilisateurs peuvent remplacer cette valeur par défaut par l'indicateur de ligne de commande « --disk-cache-dir ».

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DiskCacheDir
  - Nom de la stratégie de groupe: Définir le répertoire du cache du disque
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DiskCacheDir
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"${user_home}/Edge_cache"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DiskCacheDir
  - Exemple de valeur :
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DiskCacheSize
  #### Définir la taille de cache du disque, en octets
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configurer la taille du cache, en octets, utilisé pour stocker des fichiers sur le disque.

	Si vous activez cette stratégie, Microsoft Edge utilise la taille du cache indiquée, peu importe si l’utilisateur a spécifié l'indicateur « --disk-cache-size ». La valeur spécifiée dans cette stratégie n’est pas une délimitation fixe, mais plutôt une suggestion de système de mise en cache. Toute valeur inférieure à quelques mégaoctets est trop faible et sera arrondie au minimum raisonnable.

	Si vous définissez la valeur de cette stratégie sur 0, la taille de cache par défaut est utilisée et les utilisateurs ne peuvent pas la modifier.

	Si vous ne configurez pas cette stratégie, la taille par défaut est utilisée, mais les utilisateurs peuvent la remplacer par l'indicateur « --disk-cache-size ».

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DiskCacheSize
  - Nom de la stratégie de groupe: Définir la taille de cache du disque, en octets
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: DiskCacheSize
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x06400000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DiskCacheSize
  - Exemple de valeur :
``` xml
<integer>104857600</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DownloadDirectory
  #### Définir le répertoire de téléchargement
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configure le répertoire à utiliser lors du téléchargement de fichiers.

	Si vous activez cette stratégie, Microsoft Edge utilise le répertoire spécifié, peu importe si l’utilisateur a en spécifié un ou a choisi d'être invité à entrer l’emplacement de téléchargement à chaque fois. Voir [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) pour obtenir la liste des variables qui peuvent être utilisées.

	Si vous désactivez ou si vous ne configurez pas cette stratégie, le répertoire de téléchargement par défaut est utilisé et l’utilisateur peut modifier ce comportement.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DownloadDirectory
  - Nom de la stratégie de groupe: Définir le répertoire de téléchargement
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: DownloadDirectory
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"/home/${user_name}/Downloads"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DownloadDirectory
  - Exemple de valeur :
``` xml
<string>/home/${user_name}/Downloads</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### DownloadRestrictions
  #### Autoriser les restrictions de téléchargement
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configure le type de téléchargement que Microsoft Edge bloque complètement sans permettre aux utilisateurs de remplacer la décision de sécurité.

	Définissez « Bloquer les téléchargements dangereux » (1) de manière à autoriser tous les téléchargements, sauf ceux qui présentent des avertissements de Microsoft Defender SmartScreen.

	Définissez « Bloquer les téléchargements potentiellement dangereux » (2) de manière à autoriser tous les téléchargements, sauf ceux qui présentent des avertissements Microsoft Defender SmartScreen de téléchargements potentiellement dangereux.

	Définissez « Bloquer tous les téléchargements » (3) de manière à bloquer tous les téléchargements.

	Si vous ne configurez pas cette stratégie ou si vous définissez l'option « Pas de restriction spéciale » (0), les téléchargements passent via les restrictions de sécurité habituelles basées sur les résultats de l’analyse de Microsoft Defender SmartScreen.

	Remarque : ces restrictions s’appliquent aux téléchargements à partir du contenu de la page web, ainsi qu'à l'option de menu contextuel « lien de téléchargement... ». Ces restrictions ne s’appliquent pas à l’enregistrement ni au téléchargement de la page affichée actuellement, et ne s’appliquent pas à l’option Enregistrer au format PDF des options d’impression.

	Voir [https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934) pour plus d’informations sur Microsoft Defender SmartScreen.

	* 0 ne = Aucune restriction particulière

	* 1 = Bloquer les téléchargements dangereux

	* 2 = Bloquer les téléchargements potentiellement dangereux

	* 3 = Bloquer tous les téléchargements

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: DownloadRestrictions
  - Nom de la stratégie de groupe: Autoriser les restrictions de téléchargement
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: DownloadRestrictions
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: DownloadRestrictions
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### EdgeCollectionsEnabled
  #### Activer la fonctionnalité Collections
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Vous permet d'autoriser les utilisateurs à accéder à la fonctionnalité Collections afin de pouvoir collecter, organiser, partager et exporter du contenu de manière plus efficace et avec l'intégration d'Office.

Si vous activez ou ne configurez pas cette stratégie, les utilisateurs peuvent accéder à la fonctionnalité Collections et l'utiliser dans Microsoft Edge.

Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas accéder à la fonctionnalité Collections et ne peuvent pas l'utiliser dans Microsoft Edge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EdgeCollectionsEnabled
  - Nom de la stratégie de groupe: Activer la fonctionnalité Collections
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: EdgeCollectionsEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EdgeCollectionsEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### EditFavoritesEnabled
  #### Autorise les utilisateurs à modifier les favoris
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Activez cette stratégie pour permettre aux utilisateurs d’ajouter, de supprimer et de modifier des favoris. Il s'agit du comportement par défaut si vous ne configurez pas la stratégie.

Désactivez cette stratégie pour empêcher les utilisateurs d’ajouter, de supprimer et de modifier des favoris. Ils peuvent toujours utiliser des favoris existants.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EditFavoritesEnabled
  - Nom de la stratégie de groupe: Autorise les utilisateurs à modifier les favoris
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: EditFavoritesEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EditFavoritesEnabled
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### EnableDeprecatedWebPlatformFeatures
  #### Réactiver les fonctionnalités de plateforme web déconseillées pendant une durée limitée
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifiez la liste des fonctionnalités de plateforme web déconseillées à réactiver temporairement.

Cette stratégie vous permet de réactiver des fonctionnalités de plateforme web déconseillées pendant une durée limitée. Les fonctionnalités sont identifiées par une balise de chaîne.

Si vous ne configurez pas cette stratégie, si la liste est vide ou si une fonctionnalité ne correspond pas à l'une des balises de chaîne prises en charge, toutes les fonctionnalités de plateforme web déconseillées restent désactivées.

Alors que la stratégie proprement dite est prise en charge sur les plateformes ci-dessus, la fonctionnalité qu'elle active n’est peut-être pas disponible sur toutes ces plateformes. Toutes les fonctionnalités de plateforme web déconseillées ne peuvent pas être réactivées. Seules celles qui sont explicitement répertoriées ci-dessous peuvent être réactivées et uniquement pendant une durée limitée, qui diffère selon la fonctionnalité. Vous pouvez consulter l’intention des modifications des fonctionnalités de plateforme web à l'adresse https://bit.ly/blinkintents.

Le format général de la balise de chaîne est [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd].

* « ExampleDeprecatedFeature_EffectiveUntil20080902 » = Activer l'API ExampleDeprecatedFeature par le biais de 2008/09/02

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EnableDeprecatedWebPlatformFeatures
  - Nom de la stratégie de groupe: Réactiver les fonctionnalités de plateforme web déconseillées pendant une durée limitée
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EnableDeprecatedWebPlatformFeatures
  - Exemple de valeur :
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### EnableDomainActionsDownload
  #### Activer le téléchargement des actions de domaine à partir de Microsoft
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Dans Microsoft Edge, les actions de domaine représentent une série de fonctionnalités de compatibilité permettant au navigateur de fonctionner correctement sur le web.

Microsoft conserve la liste des actions à entreprendre sur certains domaines pour des raisons de compatibilité. Par exemple, le navigateur peut remplacer la chaîne Agent utilisateur sur un site web si ce site web a été bloqué en raison de la nouvelle chaîne Agent utilisateur dans Microsoft Edge. Chacune de ces actions est destinée à être temporaire, tandis que Microsoft tente de résoudre le problème avec le propriétaire du site.

Au démarrage du navigateur, puis régulièrement par la suite, le navigateur va contacter le service de Configuration et d'Expérimentation qui contient la liste la plus à jour des actions de compatibilité a exécuter. Cette liste est enregistrée localement une fois qu’elle a été récupérée afin que les demandes ultérieures ne mettent à jour que la liste si la copie du serveur a été modifiée.

Si vous activez cette stratégie, la liste des actions de domaine continue à être téléchargée à partir du service de Configuration et d'Expérimentation.

Si vous désactivez cette stratégie, la liste des actions de domaine n’est plus téléchargée à partir du service de Configuration et d'Expérimentation.

Si vous ne configurez pas cette stratégie, la liste des actions de domaine continue à être téléchargés à partir du service de Configuration et d'Expérimentation.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EnableDomainActionsDownload
  - Nom de la stratégie de groupe: Activer le téléchargement des actions de domaine à partir de Microsoft
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: EnableDomainActionsDownload
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EnableDomainActionsDownload
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### EnableOnlineRevocationChecks
  #### Activer les contrôles de protocole OCSP/liste de révocation de certificats en ligne
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Les vérifications de révocation en ligne ne fournissent pas un avantage de sécurité significatif et sont désactivées par défaut.

Si vous activez cette stratégie, Microsoft Edge effectue des vérifications OCSP/de liste de révocation de certificats en ligne d'erreur irrécupérable. « Erreur irrécupérable » signifie que si le serveur de révocation est inaccessible, le certificat est considéré comme valide.

Si vous désactivez la stratégie ou si vous ne la configurez pas, Microsoft Edge n’effectue pas de vérifications de révocation en ligne.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EnableOnlineRevocationChecks
  - Nom de la stratégie de groupe: Activer les contrôles de protocole OCSP/liste de révocation de certificats en ligne
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: EnableOnlineRevocationChecks
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EnableOnlineRevocationChecks
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### Autoriser les extensions managées de manière à utiliser l’API de plateforme de matériel d’entreprise
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Si cette stratégie est activée, les extensions installées par la stratégie d’entreprise sont autorisées à utiliser l’API de plateforme de matériel d’entreprise.
	Si vous désactivez cette stratégie ou ne la configurez pas, aucune extension n’est autorisée à utiliser l’API de plateforme de matériel d’entreprise.
	Cette stratégie s’applique également aux extensions de composant.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: EnterpriseHardwarePlatformAPIEnabled
  - Nom de la stratégie de groupe: Autoriser les extensions managées de manière à utiliser l’API de plateforme de matériel d’entreprise
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: EnterpriseHardwarePlatformAPIEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: EnterpriseHardwarePlatformAPIEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExperimentationAndConfigurationServiceControl
  #### Contrôler la communication avec le service d’expérimentation et de configuration
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Dans Microsoft Edge, le service d’expérimentation et de configuration permet de déployer la charge utile d’expérimentation et de configuration.

La charge utile de l’expérimentation consiste en une liste des fonctionnalités à un stade précoce de développement qui sont activées par Microsoft à des fins de test et de commentaires.

La charge utile de la configuration consiste en une liste de paramètres que Microsoft souhaite déployer pour Microsoft Edge afin d'optimiser l’expérience utilisateur. Par exemple, la charge utile de la configuration peut spécifier la fréquence à laquelle Microsoft Edge envoie des demandes au service d’expérimentation et de configuration pour récupérer la charge utile la plus récente.

Si vous définissez cette stratégie sur le mode « Récupérer les configurations et les expérimentations », la charge utile complète est téléchargée à partir du service d’expérimentation et de configuration. Cela inclut les charges utiles de l’expérimentation et celles de la configuration.

Si vous définissez cette stratégie sur le mode « Récupérer les configurations uniquement », seule la charge utile de la configuration est livrée.

Si vous définissez cette stratégie sur le mode « Désactiver la communication avec le service d’expérimentation et de configuration », la communication avec le service d’expérimentation et de configuration est complètement arrêtée.

Si vous ne configurez pas cette stratégie, sur un appareil géré sur des canaux stables et bêta, le comportement est le même qu'avec le mode « Récupérer les configurations uniquement ».

Si vous ne configurez pas cette stratégie, sur un appareil non géré, le comportement est le même qu'avec le mode « Récupérer les configurations et les expérimentations ».

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExperimentationAndConfigurationServiceControl
  - Nom de la stratégie de groupe: Contrôler la communication avec le service d’expérimentation et de configuration
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ExperimentationAndConfigurationServiceControl
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExperimentationAndConfigurationServiceControl
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### Afficher une case à cocher « Toujours ouvrir » dans la boîte de dialogue de protocole externe.
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Cette stratégie contrôle si la case à cocher « Toujours ouvrir » est affichée dans les invites de confirmation de lancement du protocole externe.

Si vous définissez cette stratégie sur True, lorsqu’une invite de confirmation de protocole externe s’affiche, l’utilisateur peut sélectionner « Toujours ouvrir ». L’utilisateur ne reçoit pas les invites de confirmation futures pour ce protocole.

Si vous définissez cette stratégie sur False ou si la stratégie n’est pas définie, la case à cocher « Toujours ouvrir » n’est pas affichée. L’utilisateur est invité à confirmer chaque fois qu’un protocole externe est appelé.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Nom de la stratégie de groupe: Afficher une case à cocher « Toujours ouvrir » dans la boîte de dialogue de protocole externe.
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### FavoritesBarEnabled
  #### Activer la barre des favoris
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active ou désactive la barre des favoris.

Si vous activez cette stratégie, les utilisateurs voient la barre des favoris.

Si vous désactivez cette stratégie, les utilisateurs ne voient pas la barre des favoris.

Si cette stratégie n’est pas configurée, l’utilisateur peut décider d’utiliser la barre des favoris ou non.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: FavoritesBarEnabled
  - Nom de la stratégie de groupe: Activer la barre des favoris
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: FavoritesBarEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: FavoritesBarEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ForceBingSafeSearch
  #### Appliquer la recherche sécurisée Bing
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Assurez-vous que les requêtes de recherche sur le web Bing sont effectuées avec la recherche sécurisée définie sur la valeur spécifiée. Les utilisateurs ne peuvent pas modifier ce paramètre.

Si vous configurez cette stratégie sur « Désactivé », la recherche sécurisée de Recherche Bing revient à la valeur bing.com.

Si vous configurez cette stratégie sur « Modéré », le paramètre modéré est utilisé dans la recherche sécurisée. Le paramètre modéré filtre les vidéos pour adultes et les images, mais pas le texte, des résultats de recherche.

Si vous configurez cette stratégie sur « Strict », le paramètre strict de la recherche sécurisée est utilisé. Le paramètre strict filtre le texte, les images et les vidéos pour adultes.

Si vous désactivez cette stratégie ou ne la configurez pas, la recherche sécurisée de Recherche Bing n’est pas appliquée et les utilisateurs peuvent définir la valeur de leur choix sur bing.com.

* 0 = Ne pas configurer de restrictions de recherche dans Bing

* 1 = Configurer des restrictions de recherche modérées dans Bing

* 2 = Configurer des restrictions de recherche strictes dans Bing

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ForceBingSafeSearch
  - Nom de la stratégie de groupe: Appliquer la recherche sécurisée Bing
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ForceBingSafeSearch
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ForceBingSafeSearch
  - Exemple de valeur :
``` xml
<integer>0</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ForceEphemeralProfiles
  #### Activer l’utilisation des profils éphémères
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôle si les profils utilisateur sont basculés en mode éphémère. Un profil éphémère est créé au début d'une session, supprimé à la fin de la session et associé au profil d’origine de l’utilisateur.

Si vous activez cette stratégie, les profils s’exécutent en mode éphémère. Cela permet aux utilisateurs de travailler à partir de leurs propres appareils sans enregistrer les données de navigation sur ces appareils. Si vous activez cette stratégie en tant que stratégie de système d'exploitation (en utilisant le GPO sous Windows, par exemple), elle s’applique à chaque profil du système.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, les utilisateurs obtiennent leur profil normal lorsqu’ils se connectent au navigateur.

En mode éphémère, les données de profil ne sont enregistrées sur le disque que pour la durée de la session utilisateur. Les fonctionnalités, telles que l’historique du navigateur, les extensions et leurs données, les données web, telles que les cookies et les bases de données web, ne sont pas enregistrées après la fermeture du navigateur. Ceci n’empêche pas les utilisateurs de télécharger manuellement des données sur le disque, ni d’enregistrer des pages ou de les imprimer. Si l’utilisateur a activé la synchronisation, toutes les données sont conservées dans leurs comptes de synchronisation, comme avec les profils normaux. Les utilisateurs peuvent également utiliser la navigation InPrivate en mode éphémère, sauf si vous désactivez explicitement cette option.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ForceEphemeralProfiles
  - Nom de la stratégie de groupe: Activer l’utilisation des profils éphémères
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ForceEphemeralProfiles
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ForceEphemeralProfiles
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ForceGoogleSafeSearch
  #### Appliquer Google SafeSearch
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Force l'exécution des requêtes Recherche Web Google avec la fonctionnalité SafeSearch activée et empêche les utilisateurs de modifier ce paramètre.

Si vous activez cette stratégie, la fonctionnalité SafeSearch de Recherche Google est toujours active.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, la fonctionnalité SafeSearch de Recherche Google n’est pas appliquée.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ForceGoogleSafeSearch
  - Nom de la stratégie de groupe: Appliquer Google SafeSearch
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ForceGoogleSafeSearch
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ForceGoogleSafeSearch
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ForceNetworkInProcess
  #### Forcer le code de mise en réseau à s’exécuter dans le processus du navigateur
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Cette stratégie force l'exécution du code réseaux dans le processus du navigateur.

Cette stratégie est désactivée par défaut et, si elle est activée, les utilisateurs risquent d'être confrontés à des problèmes de sécurité une fois le processus réseaux isolé.

Cette stratégie est conçue pour offrir aux entreprises une occasion de migrer vers des logiciels tiers qui ne dépendent pas du raccordement des API réseaux. Les serveurs proxy sont recommandés via la mise à jour corrective des API LSP et Win32.

Si cette stratégie n’est pas définie, le code réseaux peut manquer de processus navigateur en fonction des essais sur le terrain de l’expérience NetworkService.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ForceNetworkInProcess
  - Nom de la stratégie de groupe: Forcer le code de mise en réseau à s’exécuter dans le processus du navigateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ForceNetworkInProcess
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ForceYouTubeRestrict
  #### Forcer le mode Limité YouTube minimal
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Applique un mode Limité minimal à YouTube et empêche les utilisateurs de sélectionner un mode limité inférieur.

Définissez sur Strict (2) pour appliquer le mode Limité strict à YouTube.

Définissez sur Modéré (1) pour autoriser l’utilisateur à n’utiliser que les modes Limité modéré et Limité strict à YouTube. Il ne peut pas désactiver le mode Limité.

Définissez sur Désactivé (0) ou ne configurez pas cette stratégie pour ne pas appliquer le mode Limité à YouTube. Les stratégies externes, telles que les stratégies YouTube, peuvent encore appliquer le mode Limité.

* 0 = Ne pas appliquer le mode Limité sur YouTube

* 1 = Appliquer au moins le mode Limité modéré à YouTube

* 2 = Appliquer le mode Limité strict à YouTube

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ForceYouTubeRestrict
  - Nom de la stratégie de groupe: Forcer le mode Limité YouTube minimal
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ForceYouTubeRestrict
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ForceYouTubeRestrict
  - Exemple de valeur :
``` xml
<integer>0</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### FullscreenAllowed
  #### Autoriser le mode plein écran
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure

  #### Description
  Définissez la disponibilité du mode plein écran : la totalité de l'IU Microsoft Edge est masquée et seul le contenu web est visible.

	Si vous activez cette stratégie ou si vous ne la configurez pas, l’utilisateur, les applications et les extensions avec les autorisations appropriées peuvent passer en mode plein écran.

	Si vous désactivez cette stratégie, les utilisateurs, les applications et les extensions ne peuvent pas passer en mode plein écran.

	L’ouverture de Microsoft Edge en mode plein écran à l’aide de la ligne de commande n’est pas disponible lorsque le mode plein écran est désactivé.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: FullscreenAllowed
  - Nom de la stratégie de groupe: Autoriser le mode plein écran
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: FullscreenAllowed
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### Force la navigation directe sur un site intranet au lieu de rechercher des entrées à mots uniques dans la barre d’adresses
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Si vous activez cette stratégie, le premier résultat de la suggestion automatique dans la liste de suggestions de la barre d’adresses navigue vers les sites intranet si le texte entré dans la barre d’adresses est un mot unique sans ponctuation.

La navigation par défaut lors de la saisie d’un mot unique sans ponctuation effectue une navigation vers un site intranet correspondant au texte entré.

Si vous activez cette stratégie, le deuxième résultat de la suggestion automatique dans la liste de suggestions de la barre d’adresses mène à une recherche sur le web exactement telle qu’elle a été entrée, à condition que ce texte ne comporte qu’un seul mot sans ponctuation. Le moteur de recherche par défaut est utilisé, sauf si une stratégie empêchant la recherche sur le web a également été activée.

L'activation de cette stratégie peut avoir deux effets :

La navigation vers les sites en réponse à des requêtes avec un seul mot se concentrant sur un seul élément de l'historique n'apparaît plus. Au lieu de cela, le navigateur tente de naviguer vers des sites internes qui n'existent peut-être plus dans le réseau intranet d'une organisation. Cette action génère une erreur 404.

Les termes de recherche populaires à mot unique nécessitent une sélection manuelle des suggestions de recherche pour mener une recherche de manière correcte.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Nom de la stratégie de groupe: Force la navigation directe sur un site intranet au lieu de rechercher des entrées à mots uniques dans la barre d’adresses
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### HSTSPolicyBypassList
  #### Configurez la liste des noms qui vont contourner la vérification de stratégie HSTS
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Les noms d’hôte spécifiés dans cette liste seront dispensés de la vérification de stratégie HSTS qui pourrait éventuellement mettre à niveau les demandes de « http:// » vers « https:// ». Seuls les noms d’hôte en une seule partie sont autorisés dans cette stratégie. Les noms d’hôte doivent être au format canonique. Toutes les IDN doivent être convertis au format d'étiquette A et toutes les lettres ASCII doivent être en minuscule. Cette stratégie ne s’applique qu’aux noms d’hôte spécifiques indiqués ; elle ne s’applique pas aux sous-domaines des noms de la liste.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: HSTSPolicyBypassList
  - Nom de la stratégie de groupe: Configurez la liste des noms qui vont contourner la vérification de stratégie HSTS
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: HSTSPolicyBypassList
  - Exemple de valeur :
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### HardwareAccelerationModeEnabled
  #### Utiliser l’accélération matérielle (si disponible)
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifiez s'il convient d'utiliser l’accélération matérielle, si elle est disponible. Si vous activez cette stratégie ou si vous ne la configurez pas, l’accélération matérielle est activée, sauf si une fonctionnalité GPU est explicitement bloquée.

Si vous désactivez cette stratégie, l’accélération matérielle est désactivée.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: HardwareAccelerationModeEnabled
  - Nom de la stratégie de groupe: Utiliser l’accélération matérielle (si disponible)
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: HardwareAccelerationModeEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: HardwareAccelerationModeEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportAutofillFormData
  #### Autoriser l’importation des données du formulaire de remplissage auto
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer des données de formulaire de remplissage auto à partir d’un autre navigateur dans Microsoft Edge.

	Si vous activez cette stratégie, l’option d’importation manuelle des données de remplissage auto est automatiquement sélectionnée.

	Si vous désactivez cette stratégie, les données de remplissage auto ne sont pas importées lors de la première exécution et les utilisateurs ne peuvent pas les importer manuellement.

	Si vous ne configurez pas cette stratégie, les données de remplissage auto sont importées lors de la première exécution et les utilisateurs peuvent choisir d’importer ou non ces données manuellement lors des sessions de navigation ultérieures.

	Vous pouvez définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe les données de remplissage auto lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désactiver l’option **données de remplissage auto** pendant l’importation manuelle.

	**Remarque** : cette stratégie gère actuellement l’importation à partir de Google Chrome (sous Windows 7, 8 et 10 et sous macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportAutofillFormData
  - Nom de la stratégie de groupe: Autoriser l’importation des données du formulaire de remplissage auto
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportAutofillFormData
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportAutofillFormData
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportBrowserSettings
  #### Autoriser l’importation des paramètres du navigateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer les paramètres du navigateur à partir d’un autre navigateur dans Microsoft Edge.

Si vous activez cette stratégie, la case **Paramètres du navigateur** est automatiquement cochée dans la boîte de dialogue **Importer des données du navigateur**.

Si vous désactivez cette stratégie, les paramètres du navigateur ne sont pas importés lors de la première exécution et les utilisateurs ne peuvent pas les importer manuellement.

Si vous ne configurez pas cette stratégie, les paramètres du navigateur sont importés lors de la première exécution et les utilisateurs peuvent choisir s’ils souhaitent les importer manuellement lors des sessions de navigation ultérieures.

Vous pouvez également définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe les paramètres lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désactiver l’option **Paramètres du navigateur** pendant l’importation manuelle.

**Remarque** : cette stratégie gère actuellement l’importation de Google Chrome (sous Windows 7, 8 et 10 et sous macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportBrowserSettings
  - Nom de la stratégie de groupe: Autoriser l’importation des paramètres du navigateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportBrowserSettings
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportBrowserSettings
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportFavorites
  #### Autoriser l’importation des favoris
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer les favoris à partir d’un autre navigateur dans Microsoft Edge.

	Si vous activez cette stratégie, la case à cocher **Favoris** est automatiquement activée dans la boîte de dialogue **Importer des données du navigateur**.

	Si vous désactivez cette stratégie, les favoris ne sont pas importés lors de la première exécution et les utilisateurs ne peuvent pas les importer manuellement.

	Si vous ne configurez pas cette stratégie, les favoris sont importés lors de la première exécution et les utilisateurs peuvent décider de les importer manuellement lors des sessions de navigation ultérieures.

	Vous pouvez également définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe les favoris lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désactiver l’option **Favoris** pendant l’importation manuelle.

	**Remarque** : cette stratégie gère actuellement l’importation à partir d’Internet Explorer (sous Windows 7, 8 et 10), de Google Chrome (sous Windows 7, 8 et 10, et sur macOS) et des navigateurs Apple Safari (sous macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportFavorites
  - Nom de la stratégie de groupe: Autoriser l’importation des favoris
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportFavorites
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportFavorites
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportHistory
  #### Autoriser l’importation de l’historique de navigation
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer leur historique de navigation à partir d’un autre navigateur dans Microsoft Edge.

	Si vous activez cette stratégie, la case à cocher **Historique de navigation** est automatiquement activée dans la boîte de dialogue **Importer des données du navigateur**.

	Si vous désactivez cette stratégie, les données de l’historique de navigation ne sont pas importées lors de la première exécution et les utilisateurs ne peuvent pas importer ces données manuellement.

	Si vous ne configurez pas cette stratégie, les données de l’historique de navigation sont importées lors de la première exécution et les utilisateurs peuvent décider de les importer manuellement lors des sessions de navigation ultérieures.

	Vous pouvez également définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe l’historique de navigation lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désactiver l’option **Historique** pendant l’importation manuelle.

	**Remarque** : cette stratégie gère actuellement l’importation à partir d’Internet Explorer (sous Windows 7, 8 et 10), de Google Chrome (sous Windows 7, 8 et 10, et sur macOS) et des navigateurs Apple Safari (macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportHistory
  - Nom de la stratégie de groupe: Autoriser l’importation de l’historique de navigation
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportHistory
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportHistory
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportHomepage
  #### Autoriser l’importation des paramètres de la page d’accueil
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer leur paramètre de page d’accueil à partir d’un autre navigateur dans Microsoft Edge.

	Si vous activez cette stratégie, l’option d’importation manuelle du paramètre de page d’accueil est automatiquement sélectionnée.

	Si vous désactivez cette stratégie, le paramètre de la page d’accueil n’est pas importé lors de la première exécution et les utilisateurs ne peuvent pas l’importer manuellement.

	Si vous ne configurez pas cette stratégie, la page d’accueil est importée lors de la première exécution et les utilisateurs peuvent choisir d’importer ou non ces données manuellement lors des sessions de navigation ultérieures.

	Vous pouvez définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe le paramètre de page d’accueil lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désactiver l’option **page d’accueil** pendant l’importation manuelle.

	**Remarque** : cette stratégie gère actuellement l’importation à partir d’Internet Explorer (sous Windows 7, 8 et 10).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportHomepage
  - Nom de la stratégie de groupe: Autoriser l’importation des paramètres de la page d’accueil
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ImportHomepage
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportHomepage
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportOpenTabs
  #### Autoriser l’importation des onglets ouverts
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer les onglets ouverts et épinglés à partir d’un autre navigateur dans Microsoft Edge.

Si vous activez cette stratégie, la case **Onglets ouverts** est automatiquement cochée dans la boîte de dialogue **Importer des données du navigateur**.

Si vous désactivez cette stratégie, les onglets ouverts ne sont pas importés lors de la première exécution et les utilisateurs ne peuvent pas les importer manuellement.

Si vous ne configurez pas cette stratégie, les onglets ouverts sont importés lors de la première exécution et les utilisateurs peuvent choisir s’ils souhaitent les importer manuellement lors des sessions de navigation ultérieures.

Vous pouvez également définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe les onglets ouverts lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désactiver l’option **Onglets ouverts** pendant l’importation manuelle.

**Remarque** : cette stratégie ne prend actuellement en charge que l’importation à partir de Google Chrome (sous Windows 7, 8 et 10 et sous macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportOpenTabs
  - Nom de la stratégie de groupe: Autoriser l’importation des onglets ouverts
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportOpenTabs
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportOpenTabs
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportPaymentInfo
  #### Autoriser l’importation des infos de paiement
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Autorise les utilisateurs à importer des infos de paiement à partir d’un autre navigateur dans Microsoft Edge.

	Si vous activez cette stratégie, la case à cocher **infos de paiement * * est automatiquement activée dans la boîte de dialogue **Importer les données du navigateur**.

	Si vous désactivez cette stratégie, les infos de paiement ne sont pas importées lors de la première exécution et les utilisateurs ne peuvent pas les importer manuellement.

	Si vous ne configurez pas cette stratégie, les infos de paiement sont importées lors de la première exécution et les utilisateurs peuvent décider de les importer manuellement lors des sessions de navigation ultérieures.

	Vous pouvez également définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe les infos de paiement lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désélectionner l’option **infos de paiement** pendant l’importation manuelle.

	**Remarque :** cette stratégie gère actuellement l’importation à partir de Google Chrome (sous Windows 7, 8 et 10 et sous macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportPaymentInfo
  - Nom de la stratégie de groupe: Autoriser l’importation des infos de paiement
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportPaymentInfo
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportPaymentInfo
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportSavedPasswords
  #### Autoriser l’importation des mots de passe enregistrés
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer les mots de passe enregistrés à partir d’un autre navigateur dans Microsoft Edge.

	Si vous activez cette stratégie, l’option d’importation manuelle des mots de passe enregistrés est automatiquement sélectionnée.

	Si vous désactivez cette stratégie, les mots de passe enregistrés ne sont pas importés lors de la première exécution et les utilisateurs ne peuvent pas les importer manuellement.

	Si vous ne configurez pas cette stratégie, les mots de passe sont importés lors de la première exécution et les utilisateurs peuvent choisir s’ils souhaitent les importer manuellement lors des sessions de navigation ultérieures.

	Vous pouvez définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe les mots de passe lors de la première exécution, mais les utilisateurs peuvent activer ou désactiver l’option **mots de passe** pendant l’importation manuelle.

	**Remarque** : cette stratégie gère actuellement l’importation à partir d’Internet Explorer (sous Windows 7, 8 et 10) et de Google Chrome (sous Windows 7, 8 et 10 et sur macOS).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportSavedPasswords
  - Nom de la stratégie de groupe: Autoriser l’importation des mots de passe enregistrés
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportSavedPasswords
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportSavedPasswords
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ImportSearchEngine
  #### Autoriser l’importation des paramètres du moteur de recherche
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet aux utilisateurs d’importer les paramètres du moteur de recherche à partir d’un autre navigateur dans Microsoft Edge.

	Si vous activez cette stratégie, l’option permettant d’importer les paramètres du moteur de recherche est automatiquement sélectionnée.

	Si vous désactivez cette stratégie, les paramètres du moteur de recherche ne sont pas importés lors de la première exécution et les utilisateurs ne peuvent pas les importer manuellement.

	Si vous ne configurez pas cette stratégie, les paramètres du moteur de recherche sont importés lors de la première exécution et les utilisateurs peuvent choisir d’importer ou non ces données manuellement lors des sessions de navigation ultérieures.

	Vous pouvez définir cette stratégie comme une recommandation. Cela signifie que Microsoft Edge importe les paramètres du moteur de recherche lors de la première exécution, mais que les utilisateurs peuvent sélectionner ou désactiver l’option **moteur de recherche** pendant l’importation manuelle.

	**Remarque** : cette stratégie gère actuellement l’importation à partir d’Internet Explorer (sous Windows 7, 8 et 10).

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ImportSearchEngine
  - Nom de la stratégie de groupe: Autoriser l’importation des paramètres du moteur de recherche
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ImportSearchEngine
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ImportSearchEngine
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### InPrivateModeAvailability
  #### Configurer la disponibilité du mode InPrivate
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie si l’utilisateur peut ouvrir des pages en mode InPrivate dans Microsoft Edge.

	Si vous ne configurez cette stratégie ou si vous la définissez sur « Activé » (0), les utilisateurs peuvent ouvrir des pages en mode InPrivate.

	Définissez cette stratégie sur « Désactiver » (1) pour empêcher les utilisateurs d’utiliser le mode InPrivate.

	Définissez cette stratégie sur « Forcée » (2) pour toujours utiliser le mode InPrivate.

	* 0 = Mode InPrivate disponible

	* 1 = Mode InPrivate désactivé

	* 2 = Mode InPrivate forcé

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: InPrivateModeAvailability
  - Nom de la stratégie de groupe: Configurer la disponibilité du mode InPrivate
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: InPrivateModeAvailability
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: InPrivateModeAvailability
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### InternetExplorerIntegrationLevel
  #### Configurer l’intégration d’Internet Explorer
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure

  #### Description
  Pour obtenir des instructions sur la configuration optimale de l’expérience pour Internet Explorer, consultez [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: InternetExplorerIntegrationLevel
  - Nom de la stratégie de groupe: Configurer l’intégration d’Internet Explorer
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: InternetExplorerIntegrationLevel
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### InternetExplorerIntegrationSiteList
  #### Configurer la liste des sites en Mode entreprise
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Pour obtenir des instructions sur la configuration optimale de l’expérience pour Internet Explorer, consultez [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: InternetExplorerIntegrationSiteList
  - Nom de la stratégie de groupe: Configurer la liste des sites en Mode entreprise
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: InternetExplorerIntegrationSiteList
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### InternetExplorerIntegrationSiteRedirect
  #### Spécifier le type de comportement des navigations « entre les pages » vers des sites non configurés lorsqu’elles commencent sur des pages en mode Internet Explorer
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 79 ou ultérieure

  #### Description
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

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: InternetExplorerIntegrationSiteRedirect
  - Nom de la stratégie de groupe: Spécifier le type de comportement des navigations « entre les pages » vers des sites non configurés lorsqu’elles commencent sur des pages en mode Internet Explorer
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: InternetExplorerIntegrationSiteRedirect
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### IsolateOrigins
  #### Activer l’isolation de site pour des origines spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Specify origins to run in isolation, in their own process.
This policy also isolates origins named by subdomains - for example, specifying https://contoso.com/ will cause https://foo.contoso.com/ to be isolated as part of the https://contoso.com/ site.
If the policy is enabled, each of the named origins in a comma-separated list will run in its own process.
If you disable this policy, then both the 'IsolateOrigins' and 'SitePerProcess' features are disabled. Users can still enable 'IsolateOrigins' policy manually, via command line flags.
If you don't configure the policy, the user can change this setting.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: IsolateOrigins
  - Nom de la stratégie de groupe: Activer l’isolation de site pour des origines spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: IsolateOrigins
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: IsolateOrigins
  - Exemple de valeur :
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ManagedFavorites
  #### Configurer les favoris
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configurer une liste de favoris gérés.

	La stratégie crée une liste de favoris. Chaque favori contient les clés « nom » et « URL », qui contiennent le nom du favori et sa cible. Vous pouvez configurer un sous-dossier en définissant un favori sans clé « URL », mais avec une clé supplémentaire « enfants » qui contient une liste de favoris définie ci-dessus (certains peuvent être de nouveau des dossiers). Microsoft Edge modifie les URL incomplètes comme si elles étaient envoyées par le biais de la barre d'adresses, par exemple, « microsoft.com » devient « https://microsoft.com/ ».

	Ces favoris sont placés dans un dossier qui ne peut pas être modifié par l’utilisateur (mais l’utilisateur peut choisir de le masquer dans la barre des favoris). Par défaut, le nom du dossier est « Favoris gérés », mais vous pouvez le modifier en ajoutant à la liste des favoris un dictionnaire contenant la clé « toplevel_name » avec le nom de dossier souhaité comme valeur.

	Les favoris gérés ne sont pas synchronisés avec le compte d’utilisateur et ne peuvent pas être modifiés par des extensions.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ManagedFavorites
  - Nom de la stratégie de groupe: Configurer les favoris
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ManagedFavorites
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
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


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ManagedFavorites
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ManagedSearchEngines
  #### Gérer les moteurs de recherche
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Lets you configure a list of list of up to 10 search engines, one of which must be marked as the default search engine.
You do not need to specify the encoding for any search engine.

If you enable this policy, users can't add, remove, or change any search engine in the list. Users can set their default search engine to any search engine in the list.

If you disable or don't configure this policy, users can modify the search engines list as desired.

If the [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policy is set, this policy (ManagedSearchEngines) is ignored. The user must restart their browser to finish applying this policy.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Dictionnaire

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ManagedSearchEngines
  - Nom de la stratégie de groupe: Gérer les moteurs de recherche
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ManagedSearchEngines
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
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


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ManagedSearchEngines
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### MaxConnectionsPerProxy
  #### Nombre maximal de connexions simultanées au serveur proxy
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie le nombre maximal de connexions simultanées au serveur proxy.

Certains serveurs proxy ne peuvent pas gérer un nombre élevé de connexions simultanées par client. Vous pouvez résoudre ce problème en définissant cette stratégie sur une valeur inférieure.

La valeur de cette stratégie doit être inférieure à 100 et supérieure à 6. La valeur par défaut est 32.

Certaines applications web sont connues pour consommer de nombreuses connexions lors du blocage d'opérations GET. Diminuer le nombre maximal de connexions à une valeur inférieure à 32 peut bloquer les réseaux du navigateur en cas d'ouverture d'un trop grand nombre de ce type d’applications web.

Si vous ne configurez pas cette stratégie, la valeur par défaut (32) est utilisée.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: MaxConnectionsPerProxy
  - Nom de la stratégie de groupe: Nombre maximal de connexions simultanées au serveur proxy
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: MaxConnectionsPerProxy
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000020
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: MaxConnectionsPerProxy
  - Exemple de valeur :
``` xml
<integer>32</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### MediaRouterCastAllowAllIPs
  #### Autoriser Google Cast à se connecter aux appareils Cast sur toutes les adresses IP
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Enable this policy to let Google Cast connect to Cast devices on all IP addresses, not just RFC1918/RFC4193 private addresses.

Disable this policy to restrict Google Cast to Cast devices on RFC1918/RFC4193 private addresses.

If you don't configure this policy, Google Cast connects to Cast devices on RFC1918/RFC4193 private addresses only, unless you enable the CastAllowAllIPs feature.

If the [EnableMediaRouter](#enablemediarouter) policy is disabled, then this policy has no effect.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: MediaRouterCastAllowAllIPs
  - Nom de la stratégie de groupe: Autoriser Google Cast à se connecter aux appareils Cast sur toutes les adresses IP
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: MediaRouterCastAllowAllIPs
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: MediaRouterCastAllowAllIPs
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### MetricsReportingEnabled
  #### Activer l’utilisation et les rapports de données liées à l’incident
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Pour les canaux bêta et stables Windows 10 de Microsoft Edge, une fois configurée, cette stratégie écrase le paramètre de données de diagnostic Windows pour la collection ou la non-collection des données d'utilisation et d'incident de Microsoft Edge ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

Cette stratégie vous permet de signaler à Microsoft les données d'utilisation et d'incident relatives à Microsoft Edge et empêche les utilisateurs de modifier ce paramètre.

Activez cette stratégie pour envoyer les rapports de données d'utilisation et d'incident à Microsoft. Désactivez cette stratégie pour ne pas envoyer de donnée à Microsoft. Dans les deux cas, les utilisateurs ne pourront ni modifier, ni écraser ce paramètre.

Sur les canaux bêta et stables de Windows 10, cette stratégie contrôle es données d'utilisation et d'incident. Si cette stratégie n'est pas configurée, Microsoft Edge utilisera le paramètre des données de diagnostic Windows comme paramètre par défaut.

Sur les canaux Canary et Dev de Windows 10, cette stratégie contrôle les données d'utilisation et d'indicent. Si cette stratégie n'est pas configurée, Microsoft Edge utilisera la préférence de l'utilisateur par défaut.

Sur Windows 7, 8 et sur Mac, cette stratégie contrôle les données d'utilisation et d'incident. Si cette stratégie n'est pas configurée, Microsoft Edge utilisera la préférence de l'utilisateur par défaut.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: MetricsReportingEnabled
  - Nom de la stratégie de groupe: Activer l’utilisation et les rapports de données liées à l’incident
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: MetricsReportingEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: MetricsReportingEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NetworkPredictionOptions
  #### Activer la prédiction réseau
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active les prédictions réseau et empêche les utilisateurs de modifier ce paramètre.

Contrôle la prérécupération DNS, la préconnexion TCP et SSL et le prérendu des pages web.

Si vous ne configurez pas cette stratégie, les prédictions réseau sont activées, mais l’utilisateur peut modifier ce comportement.

* 0 = Prédire les actions réseau sur n'importe quelle connexion réseau

* 2 = Ne pas prédire les actions réseau sur n’importe quelle connexion réseau

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NetworkPredictionOptions
  - Nom de la stratégie de groupe: Activer la prédiction réseau
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: NetworkPredictionOptions
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: NetworkPredictionOptions
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### NonRemovableProfileEnabled
  #### Configurer si un utilisateur dispose toujours d’un profil par défaut connecté automatiquement avec son compte professionnel ou scolaire
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Cette stratégie détermine si le profil Microsoft Edge connecté automatiquement avec le compte professionnel ou scolaire d’un utilisateur peut être supprimé.

Si vous activez cette stratégie ou si vous ne la configurez pas, un profil impossible à supprimer est créé avec le compte professionnel ou scolaire de l’utilisateur sous Windows. Ce profil ne peut pas être déconnecté ni supprimé.

Si vous désactivez cette stratégie, le profil connecté automatiquement avec le compte professionnel ou scolaire d’un utilisateur à partir de Windows peut être déconnecté ou supprimé par l’utilisateur.

Si vous souhaitez désactiver complètement la connexion du navigateur, utilisez la stratégie « BrowserSignIn ».

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: NonRemovableProfileEnabled
  - Nom de la stratégie de groupe: Configurer si un utilisateur dispose toujours d’un profil par défaut connecté automatiquement avec son compte professionnel ou scolaire
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: NonRemovableProfileEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### Contrôler l’application des restrictions de sécurité aux origines non sécurisées
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie la liste des origines (URL) ou des modèles de nom d’hôte (tels que « *.contoso.com ») pour lesquels des restrictions de sécurité ne s’appliquent pas.

Cette stratégie vous permet de spécifier des origines autorisées pour les applications héritées qui ne peuvent pas déployer TLS ni définir de serveur de gestion intermédiaire pour le développement web interne afin que les développeurs puissent tester les fonctions nécessitant des contextes de sécurité sans devoir déployer TLS sur le serveur de gestion intermédiaire. Cette stratégie empêche également l’origine d'être étiquetée « Non sécurisé » dans l’omnibox.

La définition d’une liste d’URL dans cette stratégie a le même effet que la définition de l’indicateur de ligne de commande « --unsafely-treat-insecure-origin-as-secure » dans une liste d'URL identiques séparées par des virgules. Si vous activez cette stratégie, elle remplace l’indicateur de ligne de commande.

Cette stratégie remplace la stratégie « UnsafelyTreatInsecureOriginAsSecure », le cas échéant.

Pour plus d’informations sur les contextes de sécurité, voir https://www.w3.org/TR/secure-contexts/.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: OverrideSecurityRestrictionsOnInsecureOrigin
  - Nom de la stratégie de groupe: Contrôler l’application des restrictions de sécurité aux origines non sécurisées
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: OverrideSecurityRestrictionsOnInsecureOrigin
  - Exemple de valeur :
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ProactiveAuthEnabled
  #### Activer l’authentification proactive
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Vous permet de configurer l'activation et la désactivation de l'Authentification proactive.

	Si vous activez cette stratégie, Microsoft Edge tente d'authentifier de manière proactive l'utilisateur connecté aux services Microsoft. À intervalles réguliers, Microsoft Edge recherche sur le service en ligne un manifeste mis à jour contenant la configuration régissant ce comportement.

	Si vous désactivez cette stratégie, Microsoft Edge ne tente pas d'authentifier de manière proactive l'utilisateur connecté aux services Microsoft. Microsoft Edge ne recherche pas sur le service en ligne un manifeste mis à jour contenant la configuration régissant ce comportement.

	Si vous ne configurez pas cette stratégie, l'authentification proactive est activée.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ProactiveAuthEnabled
  - Nom de la stratégie de groupe: Activer l’authentification proactive
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ProactiveAuthEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ProactiveAuthEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PromotionalTabsEnabled
  #### Autoriser le contenu promotionnel dans des onglets
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Contrôler la présentation de contenu pédagogique ou promotionnel dans des onglets. Ce paramètre contrôle la présentation des pages d’accueil qui aident les utilisateurs à se connecter à Microsoft Edge, à choisir leur navigateur par défaut ou à en savoir plus sur les fonctionnalités du produit.

	Si vous activez cette stratégie (définie sur true) ou si vous ne la configurez pas, Microsoft Edge peut afficher le contenu dans des onglets pour fournir des informations sur le produit.

	Si vous désactivez (définissez sur false) cette stratégie, Microsoft Edge ne peut pas afficher le contenu dans des onglets aux utilisateurs.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PromotionalTabsEnabled
  - Nom de la stratégie de groupe: Autoriser le contenu promotionnel dans des onglets
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: PromotionalTabsEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PromotionalTabsEnabled
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### PromptForDownloadLocation
  #### Demander où enregistrer les fichiers téléchargés
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Définissez s’il faut demander où enregistrer un fichier avant de le télécharger.

Si vous activez cette stratégie, l’utilisateur est invité à indiquer l'emplacement d’enregistrement de chaque fichier avant le téléchargement. Si vous ne la configurez pas, les fichiers sont enregistrés automatiquement à l’emplacement par défaut, sans demander à l’utilisateur.

Si vous ne configurez pas cette stratégie, l’utilisateur peut modifier ce paramètre.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: PromptForDownloadLocation
  - Nom de la stratégie de groupe: Demander où enregistrer les fichiers téléchargés
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: PromptForDownloadLocation
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: PromptForDownloadLocation
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### QuicAllowed
  #### Autoriser le protocole QUIC
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Permet d’utiliser le protocole QUIC Microsoft Edge.

	Si vous activez cette stratégie ou ne la configurez pas, le protocole QUIC est autorisé.

	Si vous désactivez cette stratégie, le protocole QUIC est bloqué.

	QUIC est un protocole réseau de couche transport qui peut améliorer les performances des applications web qui utilisent TCP.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: QuicAllowed
  - Nom de la stratégie de groupe: Autoriser le protocole QUIC
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: QuicAllowed
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: QuicAllowed
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RelaunchNotification
  #### Avertir un utilisateur qu’un redémarrage du navigateur est recommandé ou requis pour les mises à jour en attente
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Notify users that they need to restart Microsoft Edge to apply a pending update.

If you don't configure this policy, Microsoft Edge adds a recycle icon at the far right of the top menu bar to prompt users to restart the browser to apply the update.

If you enable this policy and set it to 'Recommended' (1), a recurring warning prompts users that a restart is recommended. Users can dismiss this warning and defer the restart.

If you set the policy to 'Required' (2), a recurring warning prompts users that the browser will be restarted automatically as soon as a notification period passes. The default period is seven days. You can configure this period with the [RelaunchNotificationPeriod](#relaunchnotificationperiod) policy.

The user's session is restored when the browser restarts.

* Recommended (1) = Show a recurring prompt to the user indicating that a restart is recommended

* Required (2) = Show a recurring prompt to the user indicating that a restart is required

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RelaunchNotification
  - Nom de la stratégie de groupe: Avertir un utilisateur qu’un redémarrage du navigateur est recommandé ou requis pour les mises à jour en attente
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: RelaunchNotification
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: RelaunchNotification
  - Exemple de valeur :
``` xml
<integer>1</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RelaunchNotificationPeriod
  #### Définir la période pour les notifications de mise à jour
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Sets the time period, in milliseconds, over which users are notified that Microsoft Edge must be restarted to apply a pending update.

During this time period, the user is repeatedly informed that they need to restart. The app menu changes to indicate that a restart is needed when one third of the notification period passes. When two thirds of the notification period passes, the notification changes color, and again when the full notification period has passed. Additional notifications enabled by the [RelaunchNotification](#relaunchnotification) policy follow this same schedule.

If you don't configure this policy, the default period is 604800000 milliseconds (one week).

Restrictions:

* Minimum:3600000

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RelaunchNotificationPeriod
  - Nom de la stratégie de groupe: Définir la période pour les notifications de mise à jour
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: RelaunchNotificationPeriod
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x240c8400
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: RelaunchNotificationPeriod
  - Exemple de valeur :
``` xml
<integer>604800000</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RendererCodeIntegrityEnabled
  #### Activer l’intégrité du code de rendu
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Si cette stratégie est activée ou si elle est laissée non définie, l’intégrité du code de rendu est activée. Cette stratégie ne doit être désactivée que si des problèmes de compatibilité sont rencontrés avec des logiciels tiers qui doivent s’exécuter dans les processus de rendu de Microsoft Edge.

La désactivation de cette stratégie a un effet néfaste sur la sécurité et la stabilité de Microsoft Edge, car le code inconnu et potentiellement hostile est autorisé à se charger dans les processus de rendu de Microsoft Edge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RendererCodeIntegrityEnabled
  - Nom de la stratégie de groupe: Activer l’intégrité du code de rendu
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: RendererCodeIntegrityEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### Spécifier si des vérifications OCSP/liste de révocation de certificats en ligne sont obligatoires pour les ancres d’approbation locales
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure

  #### Description
  Contrôler si des vérifications de révocation en ligne (vérifications OCSP/liste de révocation de certificats) sont nécessaires. Si Microsoft Edge ne peut pas obtenir d'informations sur le statut de révocation, ces certificats sont considérés comme révoqués (« erreur irrécupérable »).

	Si vous activez cette stratégie, Microsoft Edge exécute toujours la vérification de révocation des certificats de serveur qui ont été validés et sont signés par les certificats d'autorité de certification installés localement.

	Si vous ne configurez pas ou si vous désactivez cette stratégie, Microsoft Edge utilise les paramètres de vérification de révocation en ligne existants.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RequireOnlineRevocationChecksForLocalAnchors
  - Nom de la stratégie de groupe: Spécifier si des vérifications OCSP/liste de révocation de certificats en ligne sont obligatoires pour les ancres d’approbation locales
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: RequireOnlineRevocationChecksForLocalAnchors
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ResolveNavigationErrorsUseWebService
  #### Activer la résolution des erreurs de navigation à l'aide d'un service web
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Allow Microsoft Edge to issue a dataless connection to a web service to probe networks for connectivity in cases like hotel and airport Wi-Fi.

If you enable this policy, a web service is used for network connectivity tests.

If you disable this policy, Microsoft Edge uses native APIs to try to resolve network connectivity and navigation issues.

**Note**: Except on Windows 8 and later versions of Windows, Microsoft Edge *always* uses native APIs to resolve connectivity issues.

If you don't configure this policy, Microsoft Edge respects the user preference that's set under Services at edge://settings/privacy.
Specifically, there's a **Use a web service to help resolve navigation errors** toggle, which the user can switch on or off. Be aware that if you have enabled this policy (ResolveNavigationErrorsUseWebService), the **Use a web service to help resolve navigation errors** setting is turned on, but the user can't change the setting by using the toggle. If you have disabled this policy, the **Use a web service to help resolve navigation errors** setting is turned off, and the user can't change the setting by using the toggle.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ResolveNavigationErrorsUseWebService
  - Nom de la stratégie de groupe: Activer la résolution des erreurs de navigation à l'aide d'un service web
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: ResolveNavigationErrorsUseWebService
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ResolveNavigationErrorsUseWebService
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RestrictSigninToPattern
  #### Restreindre les comptes qui peuvent être utilisés en tant que comptes principaux Microsoft Edge
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Détermine les comptes qui peuvent être définis comme comptes principaux de navigateur dans Microsoft Edge (le compte qui est choisi pendant le flux d'acceptation de synchronisation).

	Si un utilisateur tente de définir un compte principal de navigateur avec un nom d’utilisateur qui ne correspond pas à ce modèle, il est bloqué et un message d’erreur s'affiche.

	Si vous ne configurez cette stratégie ou si vous laissez le champ vide, les utilisateurs peuvent définir n’importe quel compte en tant que compte principal de navigateur dans Microsoft Edge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RestrictSigninToPattern
  - Nom de la stratégie de groupe: Restreindre les comptes qui peuvent être utilisés en tant que comptes principaux Microsoft Edge
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: RestrictSigninToPattern
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
".*@contoso.com"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: RestrictSigninToPattern
  - Exemple de valeur :
``` xml
<string>.*@contoso.com</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### RunAllFlashInAllowMode
  #### Étendre le paramètre de contenu d'Adobe Flash à l'ensemble du contenu
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  If you enable this policy, all Adobe Flash content embedded in websites that are set to allow Adobe Flash in the content settings -- either by the user or by enterprise policy -- will run. This includes content from other origins and/or small content.

To control which websites are allowed to run Adobe Flash, see the specifications in the [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls), and [PluginsBlockedForUrls](#pluginsblockedforurls) policies.

If you disable this policy or don't configure it, Adobe Flash content from other origins (from sites that aren't specified in the three policies mentioned immediately above) or small content might be blocked.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: RunAllFlashInAllowMode
  - Nom de la stratégie de groupe: Étendre le paramètre de contenu d'Adobe Flash à l'ensemble du contenu
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: RunAllFlashInAllowMode
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: RunAllFlashInAllowMode
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SSLErrorOverrideAllowed
  #### Autoriser les utilisateurs à continuer à partir de la page d’avertissement HTTPS
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Microsoft Edge affiche une page d’avertissement lorsque les utilisateurs visitent des sites présentant des erreurs SSL.

	Si vous activez cette stratégie ou ne la configurez pas (par défaut), les utilisateurs peuvent cliquer sur ces pages d’avertissement.

	Si vous désactivez cette stratégie, les utilisateurs ne peuvent cliquer sur aucune page d’avertissement.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SSLErrorOverrideAllowed
  - Nom de la stratégie de groupe: Autoriser les utilisateurs à continuer à partir de la page d’avertissement HTTPS
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SSLErrorOverrideAllowed
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SSLErrorOverrideAllowed
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SSLVersionMin
  #### Version TLS minimale activée
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Définit la version minimale prise en charge de SSL. Si vous ne configurez pas cette stratégie, Microsoft Edge utilise une version minimale par défaut, TLS 1.0.

	Si vous activez cette stratégie, vous pouvez définir la version minimale sur l’une des valeurs suivantes : « tls1 », « tls1.1 » ou « tls1.2 ». Si elle est définie, Microsoft Edge n’utilise pas une version de SSL/TLS inférieure à la version spécifiée. Une valeur non reconnue est ignorée.

	* « tls1 » = TLS 1.0

	* « tls1.1 » = TLS 1.1

	* « tls1.2 » = TLS 1.2

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SSLVersionMin
  - Nom de la stratégie de groupe: Version TLS minimale activée
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SSLVersionMin
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"tls1"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SSLVersionMin
  - Exemple de valeur :
``` xml
<string>tls1</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SavingBrowserHistoryDisabled
  #### Désactiver l’enregistrement de l’historique du navigateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Désactive l’enregistrement de l’historique du navigateur et empêche les utilisateurs de modifier ce paramètre.

Si vous activez cette stratégie, l’historique de navigation n'est pas enregistré. Ce paramètre désactive également la synchronisation des onglets.

Si vous désactivez cette stratégie ou si vous ne la configurez pas, l’historique de navigation est enregistré.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SavingBrowserHistoryDisabled
  - Nom de la stratégie de groupe: Désactiver l’enregistrement de l’historique du navigateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SavingBrowserHistoryDisabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SavingBrowserHistoryDisabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SearchSuggestEnabled
  #### Activer les suggestions de recherche
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active les suggestions de recherche sur le web dans la barre d’adresses et liste de suggestions automatiques de Microsoft Edge et empêche les utilisateurs de modifier cette stratégie.

	Si vous activez cette stratégie, les suggestions de recherche sur le web sont utilisées.

	Si vous désactivez cette stratégie, les suggestions de recherche sur le web ne sont jamais utilisées, mais l'historique local et les suggestions de favoris locaux apparaissent toujours. Si vous désactivez cette stratégie, ni les caractères tapés, ni les URL consultées ne sont inclus dans les données de télémétrie destinées à Microsoft.

	Si cette stratégie reste non définie, les suggestions de recherche sont activées, mais l’utilisateur peut modifier ce paramètre.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SearchSuggestEnabled
  - Nom de la stratégie de groupe: Activer les suggestions de recherche
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: SearchSuggestEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SearchSuggestEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SecurityKeyPermitAttestation
  #### Sites web ou domaines qui ne nécessitent pas l'autorisation d'utiliser l’attestation de clé de sécurité directe
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie les sites web et les domaines qui ne nécessitent pas d’autorisation utilisateur explicite lorsque des certificats d’attestation provenant des clés de sécurité sont obligatoires. En outre, un signal est envoyé à la clé de sécurité indiquant qu’elle peut utiliser l’attestation individuelle. Sans cela, les utilisateurs sont invités chaque fois qu’un site demande une attestation de clés de sécurité.

Les sites (par exemple, https://contoso.com/some/path) ne correspondent qu'en tant qu’appID U2F. Les domaines (par exemple, contoso.com) ne correspondent qu'en tant qu'ID RP webauthn. Pour couvrir à la fois les API U2F et webauthn pour un site donné, vous devez répertorier les domaines et URL appID.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SecurityKeyPermitAttestation
  - Nom de la stratégie de groupe: Sites web ou domaines qui ne nécessitent pas l'autorisation d'utiliser l’attestation de clé de sécurité directe
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SecurityKeyPermitAttestation
  - Exemple de valeur :
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SendIntranetToInternetExplorer
  #### Envoyer tous les sites intranet vers Internet Explorer
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure

  #### Description
  Pour obtenir des instructions sur la configuration optimale de l’expérience pour Internet Explorer, consultez [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SendIntranetToInternetExplorer
  - Nom de la stratégie de groupe: Envoyer tous les sites intranet vers Internet Explorer
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SendIntranetToInternetExplorer
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SendSiteInfoToImproveServices
  #### Envoyer les informations de site pour améliorer les services Microsoft
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Pour les canaux bêta et stables Windows 10 de Microsoft Edge, une fois configurée, cette stratégie écrase le paramètre de données de diagnostic Windows pour la collection ou la non-collection des informations de navigation de site web Microsoft Edge ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

Cette stratégie vous permet d'autoriser ou non les utilisateurs à envoyer à Microsoft des informations à propos des sites web qu'ils visitent dans Microsoft Edge afin d'améliorer certains services tels que la recherche.

Si vous activez cette stratégie, les informations relatives aux sites web visités dans Microsoft Edge sont envoyées à Microsoft.

Si vous désactivez cette stratégie, les informations relatives aux sites web visités dans Microsoft Edge ne sont pas envoyées à Microsoft.

Sur les canaux bêta et stables de Windows 10, cette stratégie contrôle l'envoi d'informations relatives aux sites web que les utilisateurs visitent. Si cette stratégie n'est pas configurée, Microsoft Edge utilisera le paramètre des données de diagnostic Windows par défaut.

Sur les canaux Canary et Dev de Windows 10, cette stratégie contrôle l'envoi d'informations relatives aux sites web que les utilisateurs visitent. Si cette stratégie n'est pas configurée, Microsoft Edge utilisera la préférence de l'utilisateur par défaut.

Sur Windows 7, 8 et sur Mac, cette stratégie contrôle l'envoi d'informations relatives aux sites web que les utilisateurs visitent. Si cette stratégie n'est pas configurée, Microsoft Edge utilisera la préférence de l'utilisateur par défaut.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SendSiteInfoToImproveServices
  - Nom de la stratégie de groupe: Envoyer les informations de site pour améliorer les services Microsoft
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SendSiteInfoToImproveServices
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SendSiteInfoToImproveServices
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### ShowOfficeShortcutInFavoritesBar
  #### Afficher les raccourcis Microsoft Office dans la barre des favoris
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifie s’il faut inclure un raccourci vers Office.com dans la barre des favoris. Pour les utilisateurs connectés à Microsoft Edge, le raccourci dirige les utilisateurs vers leurs applications et documents Microsoft Office.

	Si cette stratégie est activée ou si vous ne la configurez pas, les utilisateurs peuvent choisir d'afficher le raccourci en modifiant le bouton bascule dans le menu contextuel de la barre des favoris.

	Si vous désactivez cette stratégie, le raccourci n'est pas affiché.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: ShowOfficeShortcutInFavoritesBar
  - Nom de la stratégie de groupe: Afficher les raccourcis Microsoft Office dans la barre des favoris
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: ShowOfficeShortcutInFavoritesBar
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: ShowOfficeShortcutInFavoritesBar
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SignedHTTPExchangeEnabled
  #### Activer la prise en charge de SXG (échange HTTP signé)
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Activer le support pour Signed HTTP Exchange (SXG).

Si cette stratégie n'est pas définie ou activée, Microsoft Edge accepte les contenus web servis en tant que Signed HTTP Exchanges.

Si cette stratégie est désactivée, Signed HTTP Exchanges ne peut pas être chargé.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SignedHTTPExchangeEnabled
  - Nom de la stratégie de groupe: Activer la prise en charge de SXG (échange HTTP signé)
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SignedHTTPExchangeEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SignedHTTPExchangeEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SitePerProcess
  #### Activer l’isolation de site pour chaque site
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  The 'SitePerProcess' policy can be used to prevent users from opting out of the default behavior of isolating all sites. Note that you can also use the [IsolateOrigins](#isolateorigins) policy to isolate additional, finer-grained origins.
If you enable this policy, users can't opt out of the default behavior where each site runs in its own process.
If you disable or don’t configure this policy, a user can opt out of site isolation.  (For example, by using "Disable site isolation" entry in edge://flags.)  Disabling the policy or not configuring the policy doesn't turn off Site Isolation.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SitePerProcess
  - Nom de la stratégie de groupe: Activer l’isolation de site pour chaque site
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SitePerProcess
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SitePerProcess
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SpellcheckEnabled
  #### Activer la vérification orthographique
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  If you enable or don't configure this policy, the user can use spellcheck.

If you disable this policy, the user can't use spellcheck and the [SpellcheckLanguage](#spellchecklanguage) and [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policies are also disabled.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SpellcheckEnabled
  - Nom de la stratégie de groupe: Activer la vérification orthographique
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SpellcheckEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SpellcheckEnabled
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SpellcheckLanguage
  #### Activer des langues de vérification orthographique spécifiques
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 77 ou ultérieure

  #### Description
  Enables different languages for spellcheck. Any language that you specify that isn't recognized is ignored.

If you enable this policy, spellcheck is enabled for the languages specified, as well as any languages the user has enabled.

If you don't configure or disable this policy, there's no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is disabled, this policy will have no effect.

If a language is included in both the 'SpellcheckLanguage' and the [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policy, the spellcheck language is enabled.

The supported languages are: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SpellcheckLanguage
  - Nom de la stratégie de groupe: Activer des langues de vérification orthographique spécifiques
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SpellcheckLanguageBlocklist
  #### Forcer la désactivation des langues de la vérification orthographique
  >Versions prises en charge : Microsoft Edge sur Windows depuis la version 78 ou ultérieure

  #### Description
  Force-disables spellcheck languages. Unrecognized languages in that list will be ignored.

If you enable this policy, spellcheck will be disabled for the languages specified. The user can still enable or disable spellcheck for languages not in the list.

If you do not set this policy, or disable it, there will be no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is set to disabled, this policy will have no effect.

If a language is included in both the [SpellcheckLanguage](#spellchecklanguage) and the 'SpellcheckLanguageBlocklist' policy, the spellcheck language is enabled.

The currently supported languages are: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SpellcheckLanguageBlocklist
  - Nom de la stratégie de groupe: Forcer la désactivation des langues de la vérification orthographique
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SuppressUnsupportedOSWarning
  #### Supprimer l’avertissement de système d’exploitation non pris en charge
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Supprime l’avertissement qui s'affiche lorsque Microsoft Edge s’exécute sur un ordinateur ou un système d’exploitation qui n’est plus pris en charge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SuppressUnsupportedOSWarning
  - Nom de la stratégie de groupe: Supprimer l’avertissement de système d’exploitation non pris en charge
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: SuppressUnsupportedOSWarning
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SuppressUnsupportedOSWarning
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### SyncDisabled
  #### Désactiver la synchronisation des données à l’aide des services de synchronisation Microsoft
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Disables data synchronization in Microsoft Edge and prevents users from modifying this setting.

If this policy is not set, users will be able to either turn on or turn off sync.

Do not enable this policy when the policy 'RoamingProfileSupportEnabled' is enabled, as 'RoamingProfileSupportEnabled' duplicates the sync functionality.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: SyncDisabled
  - Nom de la stratégie de groupe: Désactiver la synchronisation des données à l’aide des services de synchronisation Microsoft
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: SyncDisabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: SyncDisabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### TabFreezingEnabled
  #### Autoriser le gel des onglets d’arrière-plan
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 79 ou ultérieure

  #### Description
  Contrôle si Microsoft Edge peut figer des onglets qui se trouvent en arrière-plan pendant au moins 5 minutes.

Le gel des onglets réduit l’utilisation de l’UC, de la batterie et de la mémoire. Microsoft Edge utilise l'heuristique pour éviter de figer des onglets qui permettent de travailler en arrière-plan, comme les notifications d’affichage, la lecture du son et la diffusion en continu de vidéo.

Si vous activez cette stratégie ou si vous ne la configurez pas, les onglets qui se trouvent à l’arrière-plan pendant au moins 5 minutes peuvent être figés.

Si vous désactivez cette stratégie, aucun onglet n’est figé.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: TabFreezingEnabled
  - Nom de la stratégie de groupe: Autoriser le gel des onglets d’arrière-plan
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: TabFreezingEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: TabFreezingEnabled
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### TaskManagerEndProcessEnabled
  #### Activer la fin des processus dans le gestionnaire des tâches du navigateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Si vous activez ou ne configurez pas cette stratégie, les utilisateurs peuvent arrêter les processus dans le Gestionnaire des tâches du navigateur. Si vous la désactivez, les utilisateurs ne peuvent pas arrêter les processus et le bouton Arrêter le processus est désactivé dans le Gestionnaire des tâches du navigateur.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: TaskManagerEndProcessEnabled
  - Nom de la stratégie de groupe: Activer la fin des processus dans le gestionnaire des tâches du navigateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: TaskManagerEndProcessEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: TaskManagerEndProcessEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### TrackingPrevention
  #### Bloquer le suivi de l’activité de navigation sur le Web des utilisateurs
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 78 ou ultérieure

  #### Description
  Vous permet de décider de bloquer les sites web effectuant le suivi des activités de navigation des utilisateurs.

Si vous activez cette stratégie, vous disposez des options suivantes pour configurer le niveau de prévention du suivi :

0 = Désactivé (aucune prévention du suivi)
1 = Basique (bloque les trackers malveillants, le contenu et les publicités seront personnalisé)
2 = Équilibré (bloque les trackers malveillants et les trackers des sites web que l'utilisateur n'a pas visité ; le contenu et les publicités seront moins personnalisés)
3 = Strict (bloque les trackers malveillants et la majorité des trackers de tous les sites ; le contenu et les publicités auront une personnalisation minimale. Certaines parties des sites pourront ne pas fonctionner)

Si vous désactivez cette stratégie ou ne la configurez pas, les utilisateurs peuvent définir leur propre niveau de prévention du suivi.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Entier

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: TrackingPrevention
  - Nom de la stratégie de groupe: Bloquer le suivi de l’activité de navigation sur le Web des utilisateurs
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: TrackingPrevention
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000002
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: TrackingPrevention
  - Exemple de valeur :
``` xml
<integer>2</integer>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### TranslateEnabled
  #### Activer Traduire
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Active le service de traduction Microsoft intégré à Microsoft Edge.

	Si vous activez cette stratégie, Microsoft Edge offre des fonctionnalités de traduction à l’utilisateur en affichant un menu volant de traduction intégré le cas échéant, et une option de traduction dans le menu contextuel.

	Désactivez cette stratégie pour désactiver toutes les fonctionnalités de traduction intégrée.

	Si vous ne configurez pas la stratégie, les utilisateurs peuvent choisir d'utiliser la fonctionnalité de traduction ou non.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Oui
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: TranslateEnabled
  - Nom de la stratégie de groupe: Activer Traduire
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): Modèles d’administration/Microsoft Edge - Paramètres par défaut (les utilisateurs peuvent les modifier)/
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): SOFTWARE\Policies\Microsoft\Edge\Recommandé
  - Nom de la valeur: TranslateEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: TranslateEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### URLAllowlist
  #### Définir une liste d’URL autorisées
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Allow access to the listed URLs, as exceptions to the URL block list.

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can use this policy to open exceptions to restrictive block lists. For example, you can include '*' in the block list to block all requests, and then use this policy to allow access to a limited list of URLs. You can use this policy to open exceptions to certain schemes, subdomains of other domains, ports, or specific paths.

The most specific filter determines if a URL is blocked or allowed. The allowed list takes precedence over the block list.

This policy is limited to 1000 entries; subsequent entries are ignored.

If you don't configure this policy, there are no exceptions to the block list in the [URLBlocklist](#urlblocklist) policy.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: URLAllowlist
  - Nom de la stratégie de groupe: Définir une liste d’URL autorisées
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: URLAllowlist
  - Exemple de valeur :
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### URLBlocklist
  #### Bloquer l’accès à une liste d’URL
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Define a list of sites, based on URL patterns, that are blocked (your users can't load them).

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can define exceptions in the [URLAllowlist](#urlallowlist) policy. These policies are limited to 1000 entries; subsequent entries are ignored.

Note that blocking internal 'edge://*' URLs isn't recommended - this may lead to unexpected errors.

This policy doesn't prevent the page from updating dynamically through JavaScript. For example, if you block 'contoso.com/abc', users might still be able to visit 'contoso.com' and click on a link to visit 'contoso.com/abc', as long as the page doesn't refresh.

If you don't configure this policy, no URLs are blocked.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: URLBlocklist
  - Nom de la stratégie de groupe: Bloquer l’accès à une liste d’URL
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
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


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: URLBlocklist
  - Exemple de valeur :
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
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### UserDataDir
  #### Définir le répertoire des données utilisateur
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Configurer le répertoire à utiliser pour le stockage des données utilisateur.

	Si vous activez cette stratégie, Microsoft Edge utilise le répertoire spécifié, peu importe si l’utilisateur a spécifié l'indicateur de ligne de commande « --user-data-dir ».

	Si vous ne configurez pas cette stratégie, le chemin d’accès du profil par défaut est utilisé et l’utilisateur peut le remplacer par l'indicateur de ligne de commande « --user-data-dir ». Le répertoire du profil est accessible par l’utilisateur dans le chemin d'accès du profil edge://version/.

	Pour éviter toute perte de données ou d’autres erreurs inattendues, ne configurez pas cette stratégie sur le répertoire racine d’un volume ni sur un répertoire utilisé à d’autres fins, car Microsoft Edge gère son contenu.

	Voir [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) pour obtenir la liste des variables qui peuvent être utilisées.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: UserDataDir
  - Nom de la stratégie de groupe: Définir le répertoire des données utilisateur
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: UserDataDir
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"${users}/${user_name}/Edge"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: UserDataDir
  - Exemple de valeur :
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### UserFeedbackAllowed
  #### Autoriser les commentaires des utilisateurs
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Microsoft Edge utilise la fonctionnalité de commentaires Edge (activée par défaut) pour permettre aux utilisateurs d’envoyer des commentaires, des suggestions ou des enquêtes client et de signaler des problèmes liés au navigateur. En outre, par défaut, les utilisateurs ne peuvent pas désactiver la fonctionnalité de commentaires Edge.

	Si vous activez cette stratégie ou ne la configurez pas, les utilisateurs peuvent appeler des commentaires Edge.

	Si vous désactivez cette stratégie, les utilisateurs ne peuvent pas invoquer les commentaires Edge.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: UserFeedbackAllowed
  - Nom de la stratégie de groupe: Autoriser les commentaires des utilisateurs
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: UserFeedbackAllowed
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: UserFeedbackAllowed
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### VideoCaptureAllowed
  #### Autoriser ou bloquer la capture vidéo
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Control whether sites can capture video.

If enabled or not configured (default), the user will be asked about video capture access for all sites except those with URLs configured in the [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy list, which will be granted access without prompting.

If you disable this policy, the user isn't prompted, and video capture is only available to URLs configured in [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy.

This policy affects all types of video inputs, not only the built-in camera.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: VideoCaptureAllowed
  - Nom de la stratégie de groupe: Autoriser ou bloquer la capture vidéo
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: VideoCaptureAllowed
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000000
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: VideoCaptureAllowed
  - Exemple de valeur :
``` xml
<false/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### VideoCaptureAllowedUrls
  #### Sites pouvant accéder aux appareils de capture vidéo sans demander l’autorisation
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Spécifiez les sites web, en fonction de modèles d’URL, qui peuvent utiliser des appareils de capture vidéo sans demander l’autorisation de l'utilisateur. Les modèles de cette liste sont comparés à l’origine de sécurité de l’URL d'incorporation. S'ils correspondent, le site reçoit automatiquement l’accès à des appareils de capture vidéo.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Oui

  #### Type de données:
  Liste de chaînes

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: VideoCaptureAllowedUrls
  - Nom de la stratégie de groupe: Sites pouvant accéder aux appareils de capture vidéo sans demander l’autorisation
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - Chemin (Recommandé): N/A
  - Nom de la valeur: 1, 2, 3, ...
  - Type de la valeur: liste de REG_SZ
  ##### Exemple de valeur :
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: VideoCaptureAllowedUrls
  - Exemple de valeur :
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### WPADQuickCheckEnabled
  #### Définir l'optimisation WPAD
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Vous autorise à désactiver l’optimisation WPAD (Découverte automatique de proxy web) dans Microsoft Edge.

	Si vous désactivez cette stratégie, l’optimisation WPAD est désactivée, ce qui fait patienter le navigateur plus longtemps que les serveurs WPAD basés sur DNS.

	Si vous activez ou ne configurez pas la stratégie, l’optimisation WPAD est activée.

	Indépendamment de l'activation ou non de cette stratégie, le paramètre d’optimisation WPAD ne peut pas être modifié par les utilisateurs.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: WPADQuickCheckEnabled
  - Nom de la stratégie de groupe: Définir l'optimisation WPAD
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: WPADQuickCheckEnabled
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: WPADQuickCheckEnabled
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### WebDriverOverridesIncompatiblePolicies
  #### Autoriser WebDriver à remplacer les stratégies incompatibles
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  This policy was removed in M80, because it is not necessary anymore as
WebDriver is now compatible with all existing policies.

This policy allows users of the WebDriver feature to override
policies which can interfere with its operation.

Currently this policy disables [SitePerProcess](#siteperprocess) and [IsolateOrigins](#isolateorigins) policies.

If the policy is enabled, WebDriver will be able to override incomaptible
policies.
If the policy is disabled or not configured, WebDriver will not be allowed
to override incompatible policies.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Booléen

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: WebDriverOverridesIncompatiblePolicies
  - Nom de la stratégie de groupe: Autoriser WebDriver à remplacer les stratégies incompatibles
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: WebDriverOverridesIncompatiblePolicies
  - Type de la valeur: REG_DWORD
  ##### Exemple de valeur :
```
0x00000001
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: WebDriverOverridesIncompatiblePolicies
  - Exemple de valeur :
``` xml
<true/>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### WebRtcLocalhostIpHandling
  #### Limiter l’exposition de l’adresse IP localhost par WebRTC
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Vous permet de définir si WebRTC expose son adresse IP localhost.

Si vous définissez cette stratégie « AllowAllInterfaces » (« default ») ou « AllowPublicAndPrivateInterfaces » (« default_public_and_private_interfaces »), WebRTC expose l’adresse IP localhost.

Si vous définissez cette stratégie sur « AllowPublicInterfaceOnly » (« default_public_interface_only ») ou « DisableNonProxiedUdp » (« disable_non_proxied_udp »), WebRTC n’expose pas l’adresse IP localhost.

Si vous ne définissez pas cette stratégie ou si vous la désactivez, WebRTC expose l’adresse IP localhost.

* « default » = Autoriser toutes les interfaces. Ceci expose l’adresse IP localhost.
* « default_public_and_private_interfaces » = autoriser les interfaces publiques et privées à l’itinéraire par défaut de http. Affichez l’adresse IP de localhost.
* « default_public_interface_only » = Autoriser l’interface publique sur l’itinéraire http par défaut. Ceci n’expose pas l’adresse IP localhost.
* « disable_non_proxied_udp » = Utiliser TCP, sauf si le serveur proxy prend en charge UDP. Ceci n’expose pas l’adresse IP localhost.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: WebRtcLocalhostIpHandling
  - Nom de la stratégie de groupe: Limiter l’exposition de l’adresse IP localhost par WebRTC
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: WebRtcLocalhostIpHandling
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"default"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: WebRtcLocalhostIpHandling
  - Exemple de valeur :
``` xml
<string>default</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)

  ### WebRtcUdpPortRange
  #### Limiter la plage de ports UDP locaux utilisés par WebRTC
  >Versions prises en charge : Microsoft Edge sur Windows et Mac depuis la version 77 ou ultérieure

  #### Description
  Limite la plage de ports UDP utilisée par WebRTC à un intervalle de ports spécifié (points de terminaison inclus).

En configurant cette stratégie, vous spécifiez la plage de ports UDP locaux que WebRTC peut utiliser.

Si vous ne configurez pas cette stratégie ou si vous définissez une chaîne vide ou une plage de ports non valide, WebRTC peut utiliser n’importe quel port UDP local disponible.

  #### Fonctionnalités prises en charge :
  - Peut être obligatoire: Oui
  - Peut être recommandé(e): Non
  - Actualisation de la stratégie dynamique: Non - Nécessite le redémarrage du navigateur

  #### Type de données:
  Chaîne

  #### Informations et paramètres Windows
  ##### Informations sur la stratégie de groupe (ADMX)
  - Nom unique de stratégie de groupe: WebRtcUdpPortRange
  - Nom de la stratégie de groupe: Limiter la plage de ports UDP locaux utilisés par WebRTC
  - Chemin d'accès à la stratégie de groupe (Obligatoire): Modèles d’administration/Microsoft Edge/
  - Chemin d'accès à la stratégie de groupe (Recommandé): N/A
  - Nom du fichier ADMX de stratégie de groupe: MSEdge.admx
  ##### Paramètres du Registre Windows
  - Chemin (Obligatoire): SOFTWARE\Policies\Microsoft\Edge
  - Chemin (Recommandé): N/A
  - Nom de la valeur: WebRtcUdpPortRange
  - Type de la valeur: REG_SZ
  ##### Exemple de valeur :
```
"10000-11999"
```


  #### Paramètres et informations Mac
  - Nom de la clé de préférence: WebRtcUdpPortRange
  - Exemple de valeur :
``` xml
<string>10000-11999</string>
```
  

  [Revenir au début](#microsoft-edge---stratégies)


## Voir aussi
- [Configuration de Microsoft Edge](configure-microsoft-edge.md)
- [Page d’arrivée de Microsoft Edge Entreprise](https://aka.ms/EdgeEnterprise)