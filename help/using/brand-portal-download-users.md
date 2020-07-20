---
title: Téléchargement de ressources
seo-title: Téléchargement de ressources
description: Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion.
seo-description: Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 100%

---


# Téléchargement de ressources {#download-assets}

Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès à partir de Brand Portal. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion. Lisez ce qui suit pour savoir comment télécharger des ressources approuvées à partir de Brand Portal et en savoir plus sur les [performances de téléchargement](../using/brand-portal-download-users.md#main-pars-header).

>[!NOTE]
>
>Seuls les administrateurs peuvent télécharger les ressources arrivées à expiration. Pour plus d’informations sur les ressources arrivées à expiration, voir [Gestion des droits numériques des ressources](../using/manage-digital-rights-of-assets.md).

## Étapes de téléchargement des ressources     {#steps-to-download-assets}

Pour télécharger des fichiers ou des dossiers contenant des ressources pour Brand Portal, procédez comme suit :

1. Dans l’interface de Brand Portal, effectuez l’une des opérations suivantes :

   * Sélectionnez les dossiers ou les ressources que vous souhaitez télécharger. Dans la barre d’outils supérieure, cliquez sur l’icône **[!UICONTROL Télécharger]**.

   ![](assets/downloadassets-1.png)

   * Pour télécharger un seul dossier ou une ressource, placez le pointeur dessus. Dans les miniatures d’action rapide disponibles, cliquez sur l’icône **[!UICONTROL Télécharger]**.

   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >Si les ressources que vous téléchargez comprennent également des ressources sous licence, vous êtes redirigé vers la page **[!UICONTROL Gestion des droits d’auteur]**. Dans cette page, sélectionnez les ressources, cliquez d&#39;abord sur **[!UICONTROL Accepter]**, puis sur **[!UICONTROL Télécharger]**. Si vous choisissez de ne pas accepter, les ressources sous licence ne sont pas téléchargées.\
   >Dans le cas des ressources protégées par une licence, un [contrat de licence leur est associé](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) en définissant la [propriété de métadonnées](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) appropriée dans AEM Assets.

   ![](assets/licensed-asset-download-1.png)

   La boîte de dialogue **[!UICONTROL Télécharger]** s’affiche avec l’option **[!UICONTROL Ressource(s)]** sélectionnée par défaut.

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >Si les ressources que vous téléchargez sont des fichiers images et si vous choisissez seulement l’option **[!UICONTROL Ressource(s)]** de la boîte de dialogue Télécharger, sans être [autorisé par l’administrateur à accéder aux rendus originaux des fichiers images](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), aucun fichier image n’est téléchargé, et un avis vous indique que l’administrateur a restreint votre accès aux rendus originaux.

   ![](assets/restrictaccess-note.png)

1. Pour télécharger les rendus des ressources en plus des ressources, sélectionnez **[!UICONTROL Rendu(s)]**. Toutefois, pour autoriser le téléchargement des rendus générés automatiquement avec des rendus personnalisés, désélectionnez l’option **[!UICONTROL Exclure les rendus générés automatiquement]**, qui est sélectionnée par défaut.

   ![](assets/exclude-auto-renditions.png)

   Pour télécharger uniquement les rendus, désélectionnez **[!UICONTROL Ressource(s)]**.

   >[!NOTE]
   >
   >Par défaut, seules les ressources sont téléchargées. Toutefois, les rendus originaux des fichiers images ne sont pas téléchargés si vous n’êtes pas [autorisé par l’administrateur à y accéder](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   * Pour accélérer le téléchargement des fichiers de ressources à partir de Brand Portal, sélectionnez l’option **[!UICONTROL Autoriser l’accélération des téléchargements]** et [suivez l’assistant](../using/accelerated-download.md#main-pars-header-405749062). Pour en savoir plus sur le téléchargement plus rapide des ressources, consultez le [Guide d’accélération des téléchargements à partir de Brand Portal](../using/accelerated-download.md).

   * Pour appliquer un [paramètre prédéfini d’image personnalisé à la ressource et ses rendus](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), sélectionnez **[!UICONTROL Rendu(s) dynamique(s)]**. Indiquez les propriétés du paramètre prédéfini d’image personnalisé (taille, format, espace colorimétrique, résolution et modificateur d’image) pour l’appliquer lors du téléchargement de la ressource et de ses rendus. Pour télécharger uniquement les rendus dynamiques, désélectionnez **[!UICONTROL Ressource(s)]**.

   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >Pour prévisualiser (ou télécharger) les rendus dynamiques d’une ressource, vérifiez que Dynamic Media est activé et que le rendu Pyramid tiff de la ressource existe au niveau de l’instance AEM Author à partir de laquelle les ressources ont été publiées. Lorsqu’une ressource est publiée sur Brand Portal, son rendu Pyramid tiff l’est également. Il n’existe aucun moyen pour générer le rendu Pyramid tiff à partir de Brand Portal.

   * Pour conserver la hiérarchie des dossiers de Brand Portal lors du téléchargement des ressources, sélectionnez **[!UICONTROL Créer un dossier distinct pour chaque ressource]**. Par défaut, la hiérarchie des dossiers de Brand Portal est ignorée, et toutes les ressources sont téléchargées dans un dossier de votre système local.

   * Pour envoyer aux utilisateurs un e-mail de notification comportant un lien pour télécharger les ressources, sélectionnez **[!UICONTROL Courrier électronique]**.

   ![](assets/download-link.png)

   >[!NOTE]
   >
   >Le lien de téléchargement figurant dans l&#39;e-mail de notification expire après 45 jours.
   >
   >Les administrateurs peuvent personnaliser les e-mails, à savoir le logo, la description et le pied de page à l’aide de la fonctionnalité [Valorisation de marque](../using/brand-portal-branding.md).

1. Cliquez sur **[!UICONTROL Télécharger]**.

   Les ressources, et les rendus s’ils sont sélectionnés, sont téléchargés en tant que fichier ZIP dans votre dossier local. Cependant, aucun fichier ZIP n’est créé lorsqu’une seule ressource est téléchargée sans aucun des rendus, assurant ainsi un téléchargement rapide.

   Les rendus originaux des ressources sélectionnées ne sont pas téléchargés si vous n’êtes pas [autorisé par l’administrateur à y accéder](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   >[!NOTE]
   >
   >Les ressources sélectionnées individuellement et téléchargées sont visibles dans le rapport sur les ressources téléchargées. Toutefois, si un dossier contenant des ressources est téléchargé, le dossier et les ressources ne sont pas affichés dans le rapport sur les ressources téléchargées.

   Pour savoir comment télécharger des ressources à partir de liens partagés, voir [Téléchargement de ressources à partir de liens partagés](../using/brand-portal-link-share.md#main-pars-header-1703469193).

## Performances de téléchargement attendues {#expected-download-performance}

L’expérience de téléchargement de fichier peut varier pour les utilisateurs situés à différents emplacements, en fonction de facteurs tels que la connexion Internet locale et la latence du serveur. Les performances de téléchargement attendues pour un fichier de 2 Go observées à différents emplacements de clients sont les suivantes, avec le serveur    Serveur Brand Portal dans l’Oregon aux États-Unis :

| Emplacement du client | Latence entre le client et le serveur | Vitesse de téléchargement prévue | Temps nécessaire pour télécharger un fichier de 2 Go |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| Ouest des États-Unis (Californie du Nord) | 18 millisecondes | 7,68 Mo/s. | 4 minutes |
| Ouest des États-Unis (Oregon) | 42 millisecondes | 3,84 Mo/s. | 9 minutes |
| Est des États-Unis (Virginie du Nord) | 85 millisecondes | 1,61 Mo/s. | 21 minutes |
| Asie-Pacifique (Tokyo) | 124 millisecondes | 1,13 Mo/s. | 30 minutes |
| Noida | 275 millisecondes | 0,5 Mo/s. | 68 minutes |
| Sydney | 175 millisecondes | 0,49 Mo/s. | 69 minutes |
| Londres | 179 millisecondes | 0,32 Mo/s. | 106 minutes |
| Singapour | 196 millisecondes | 0,5 Mo/s. | 68 minutes |

**Remarque** : les données citées sont observées dans les situations de test et peuvent varier pour des utilisateurs à des emplacements différents avec une latence et une bande passante différentes.
